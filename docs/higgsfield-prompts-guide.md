# Руководство по написанию промптов для Higgsfield.ai Ultimate
## Генерация изображений и видео

---

## Оглавление
1. [Основы структуры промптов](#основы-структуры-промптов)
2. [Формула эффективного промпта](#формула-эффективного-промпта)
3. [Motion Controls в Higgsfield](#motion-controls-в-higgsfield)
4. [Примеры промптов для разных сценариев](#примеры-промптов-для-разных-сценариев)
5. [Техники для видеопроизводства](#техники-для-видеопроизводства)
6. [Лучшие практики](#лучшие-практики)

---

## Основы структуры промптов

### Структура Text-to-Image промпта

```
[Main Subject] + [Appearance Details] + [Action/Pose] + 
[Environment] + [Lighting] + [Style] + [Mood/Emotion]
```

**Пример:**
> A desperate thief, torn dark coat, intense focused eyes, darts through a rain-soaked alley with glistening cobblestones under flickering streetlamp, cinematic noir style, tense and urgent atmosphere

---

### Структура Text-to-Video промпта (Image-to-Video)

```
[Opening Action] + [Camera Position & Movement] + 
[Environmental Interaction] + [Background Elements] + 
[Camera Effects] + [Lighting Details] + [Emotional Conclusion]
```

**Пример:**
> A desperate thief darts through a rain-soaked alley, the camera positioned low and directly behind him, following every frantic stride. Rain splatters against the cobbled pavement, sending droplets flying. Garbage bins loom on either side as he weaves past. The camera shakes slightly with each step. Dim streetlight glints off puddles. Fear and determination blend into a single exhilarating moment.

---

## Формула эффективного промпта

### Базовая формула (Universal)

```
[Camera Movement] + [Subject Motion] + [Speed] + [Visual Style] + [Quality]
```

**Пример:**
> Slow push in, character blinks and smiles softly, gentle movement, cinematic lighting, 4K quality

### Расширенная формула для Higgsfield

```
[Subject Details] + [Action/Movement] + [Camera Technique] + 
[Environment & Lighting] + [Visual Style] + [Mood] + [Resolution]
```

---

## Motion Controls в Higgsfield

### Полный список доступных motion controls в Ultimate плане

#### 1. **Dolly Controls** (Линейное движение камеры)

| Motion | Описание | Когда использовать |
|--------|---------|-------------------|
| **Dolly In** | Камера движется ближе к субъекту | Интимные моменты, фокус на деталях, откровения |
| **Dolly Out** | Камера отодвигается от субъекта | Раскрытие контекста, финалы, изоляция |
| **Dolly Left** | Камера движется влево | Отслеживание движения, переходы между элементами |
| **Dolly Right** | Камера движется вправо | Боксерский ринг, боевые сцены, динамические переходы |
| **Dolly Zoom In** | Движение ближе + зум наружу | Шок, дезориентация, психологический стресс |
| **Dolly Zoom Out** | Движение в сторону + зум внутрь | Чувство беспомощности, изоляции, подавленности |
| **Super Dolly In** | Экстремально быстрое приближение | Резкие откровения, удар, срочность |
| **Super Dolly Out** | Экстремально быстрое отдаление | Раскрытие огромного масштаба, потеря контроля |

**Промпт-пример Dolly In:**
> The old man sits clutching a faded photograph. The camera dollies in slowly, closing on his face as tears glisten in his eyes, revealing deep solitude and regret.

---

#### 2. **Crane Controls** (Вертикальное движение)

| Motion | Описание | Когда использовать |
|--------|---------|-------------------|
| **Crane Up** | Камера поднимается вверх | Откровение масштаба, переход от интима к грандиозу |
| **Crane Down** | Камера опускается вниз | Введение локации, переход к деталям |
| **Crane Over Head** | Камера движется над субъектом | Уязвимость, одиночество, божественная перспектива |

**Промпт-пример Crane Up:**
> A soldier kneels on battlefield clutching his helmet. The camera cranes up from his shaking hands, rising to reveal vast, smoky expanse of war-torn landscape with fallen comrades and flickering fires.

---

#### 3. **Circular & Orbit Controls** (Круговое движение)

| Motion | Описание | Когда использовать |
|--------|---------|-------------------|
| **360 Orbit** | Полный круг вокруг субъекта | Выделение персонажа, изоляция, психологический портрет |
| **Lazy Susan** | Медленное вращение вокруг статичного объекта | Демонстрация деталей, обзор продукта, интродакшны |

**Промпт-пример 360 Orbit:**
> A lone boxer stands in ring center, chest heaving from exhaustion. The camera orbits 360 degrees around him, capturing his sweat-soaked face from every angle. Lights blur into circular glow as camera completes arc, emphasizing his isolation in spotlight.

---

#### 4. **Arc & Sweep Controls**

| Motion | Описание | Когда использовать |
|--------|---------|-------------------|
| **Arc** | Дугообразное движение вокруг субъекта | Интенсивные разговоры, поворотные моменты, раскрытие контекста |

**Промпт-пример Arc:**
> Two detectives stand on rooftop overlooking city at dusk. The camera arcs slowly around them, shifting from their pensive faces to sprawling skyline, blending quiet conversation with hum of metropolis.

---

#### 5. **Zoom & Macro Controls**

| Motion | Описание | Когда использовать |
|--------|---------|-------------------|
| **Crash Zoom In** | Быстрый зум к субъекту | Шок, реализация, срочное внимание |
| **Crash Zoom Out** | Быстрый зум в сторону | Неожиданное раскрытие контекста, отключение |
| **Fisheye** | Искаженное, дугообразное изображение | Дезориентация, сюрреализм, экспериментальность |

**Промпт-пример Crash Zoom:**
> Detective's eyes widen spotting bloody handprint on windowsill. The camera crash zooms in on the mark, emphasizing chilling evidence against eerie silence of room.

---

#### 6. **Handheld & Documentary Controls**

| Motion | Описание | Когда использовать |
|--------|---------|-------------------|
| **Handheld** | Дрожащая, органичная камера | Хаос, интимность, реалистичность, стресс |
| **Head Tracking** | Камера следит за головой персонажа | Интроспекция, дезориентация, фокус на эмоциях |
| **Snorricam** | Камера закреплена на актере, фон движется | Экстремальный стресс, опьянение, боевые сцены |
| **Dirty Lens** | Линза испачкана/затуманена | Боевые сцены, экстремальные условия, реализм |

**Промпт-пример Handheld:**
> Protester pushes through crowd, handheld camera jostling with every shove. Chanting and body pressure surround him, shaky footage capturing chaotic energy of demonstration with raw immediacy.

---

#### 7. **Action Controls** (Специализированные движения)

| Motion | Описание | Когда использовать |
|--------|---------|-------------------|
| **Action Run** | Камера следит за бегущим персонажем | Погони, побеги, интенсивность |
| **Bullet Time** | Медленная съемка вокруг замороженного субъекта | Боевые сцены, экшн-клаймаксы, величественные моменты |
| **Car Chasing** | Следование за быстрым автомобилем | Погони, высокие скорости, экшн |
| **Car Grip** | Камера закреплена на машине | Трюки, дрифты, динамические поворты |
| **Flying** | Камера парит/скользит по воздуху | Аэрокадры, свобода, исследование |
| **FPV Drone** | Агильный дрон, квадрокоптер POV | Боевые сцены, погони, спорт |
| **Hyperlapse** | Медленное движение + ускоренное время | Переходы дня в ночь, урбанистические сцены |

**Промпт-пример Action Run:**
> Desperate thief darts through rain-soaked alley, camera positioned low behind him, following frantic stride. Rain splatters on cobblestones. Garbage bins flash past. Camera shakes with each surge forward, transmitting adrenaline-fueled panic.

---

#### 8. **Special Effects Controls**

| Motion | Описание | Когда использовать |
|--------|---------|-------------------|
| **Dutch Angle** | Наклоненная камера | Тревога, неустойчивость, психологический стресс |
| **Low Shutter** | Медленная выдержка, размытие движения | Боевые сцены, спортивные движения, интоксикация |
| **Focus Change** | Переключение фокуса между элементами | Раскрытие скрытого, переключение внимания |
| **Through Object In** | Камера проходит через объект | Переходы, раскрытие секретов, входы |
| **Through Object Out** | Камера выходит через объект | Выходы, переходы сцен, раскрытие пространства |
| **Levitation** | Плавное парение вверх | Мистика, духовность, трансценденция |
| **Mouth In** | Зум в рот персонажа | Фантазийные переходы, сновидения, начало истории |
| **Object POV** | Перспектива предмета | Комедия, уникальные углы, странные ракурсы |
| **Tentacles** | Извилистое, органичное движение | Ужас, сюрреализм, неестественность |

**Промпт-пример Dutch Angle:**
> Conspirators whisper in dimly lit room at Dutch angle, their shadows stretching across warped floor. Hinting at betrayal, deceit, and impossible alliances forming in darkness.

---

#### 9. **Combo Controls** (Комбинированные движения)

**Rap Flex**: Динамичные быстрые движения в ритм музыки
> Rapper spits bars on graffitied street corner, camera snapping forward with each verse, pulling back with beat, whipping around as crew joins in, amplifying raw energy of freestyle.

**Robo Arm**: Механически точное, плавное сложное движение
> Robotic arm swings camera in sweeping arc around sleek sports car, starting from headlights, moving up over roof, revealing cityscape reflecting on glossy finish.

**Kiss**: Мягкое приближение к интимному моменту
> Lovers lean into each other, camera dollying in smoothly as lips meet. Soft evening light filters through window, world blurs around them.

---

## Примеры промптов для разных сценариев

### 1. Видеопроизводство – Интро/Другой контент

#### Пример 1: Cinematic Intro для YouTube (16:9)
```
A sleek laptop sits on a dark desk, neon RGB lighting casting blue and purple glow. 
The camera dolly zooms in slowly, revealing code flowing on the screen in green text. 
Dust particles drift through the colored light rays. 
Style: Cinematic, moody, high-contrast. 
Camera: Dolly In + Low Shutter effect. 
Mood: Professional, focused, tech-forward.
Resolution: 1080p (16:9)
```

#### Пример 2: Product Showcase (9:16 для Reels/TikTok)
```
A gaming mouse sits centered on a clean white table. 
The camera orbits 360 degrees slowly around it, showing every angle and RGB detail. 
Soft studio lighting creates sharp, professional reflections on the matte black surface. 
Style: Product photography, clean, minimalist. 
Camera: Lazy Susan (slow 360 orbit). 
Mood: Premium, desirable, sleek.
Resolution: 720p (9:16)
```

#### Пример 3: Behind-the-Scenes (16:9)
```
A video editor sits at workstation, multiple monitors glowing. 
The camera handheld moves around them, capturing frantic clicking, keyboard typing, 
timeline scrubbing. Quick cuts between screens showing color grading and VFX. 
Style: Documentary, authentic, energetic. 
Camera: Handheld with quick focus changes. 
Mood: Creative chaos, productive intensity.
Resolution: 1080p (16:9)
```

---

### 2. AI Генерация для Видеопроизводства

#### Пример 4: Sci-Fi Scene Transition
```
A futuristic city at night, neon signs reflecting on wet streets. 
Holographic advertisements flicker above. 
The camera flies through the air as an FPV drone, weaving between skyscrapers, 
diving through neon-lit corridors. 
Flying cars zoom past in the distance.
Style: Cyberpunk, Blade Runner-inspired, high-tech neon.
Camera: FPV Drone with sharp turns and dives.
Mood: Fast-paced, dangerous, awe-inspiring.
Resolution: 720p (16:9)
Duration: 3-5 seconds
```

#### Пример 5: Emotional Character Moment
```
A woman stands alone in abandoned subway station, dust particles floating in golden afternoon light. 
Her face shows exhaustion and determination. 
The camera performs a slow 360 orbit around her, capturing her from all angles. 
Graffiti-covered walls surround her. Wind whistles through broken windows.
Style: Cinematic drama, naturalistic lighting, gritty realism.
Camera: 360 Orbit, slow and deliberate.
Mood: Solitude, resilience, hope amid despair.
Resolution: 720p (16:9)
Duration: 4 seconds
```

#### Пример 6: Action Sequence Setup
```
A parkour athlete crouches on rooftop edge, city sprawling below. 
Wind whips through their hair. 
They leap forward and the camera follows in FPV drone mode, 
cutting through air as they soar above traffic and buildings below.
Style: Action cinema, dynamic, adrenaline-pumping.
Camera: FPV Drone + Action Run hybrid.
Mood: Extreme energy, triumph, defiance.
Resolution: 720p (16:9)
Duration: 3 seconds
```

---

### 3. Примеры для Fallout Модов / Геймпрей

#### Пример 7: Fallout Character Intro
```
A weathered vault dweller in pre-war armor stands in post-apocalyptic wasteland, 
Sunset bleeds orange and red across irradiated sky. 
Broken buildings silhouette against sky. 
The camera starts low, positioned behind the vault dweller, 
then slowly cranes up to reveal the vast, desolate landscape. 
Dust devils swirl in the distance.
Style: Retro-futuristic, gritty, desolate, VHS-like degradation.
Camera: Crane Up from low angle.
Mood: Lonely, determined, post-apocalyptic.
Resolution: 720p (16:9)
Duration: 4 seconds
```

#### Пример 8: Weapon Showcase
```
A vintage plasma rifle sits on weathered workbench surrounded by scrap parts. 
Energy cells glow softly beside it. 
The camera orbits slowly around the weapon, showing intricate details, 
glowing core, and battle-worn scratches. 
Blue neon underglow illuminates the bench.
Style: Retro-futuristic, industrial, neon accents, slightly aged.
Camera: Lazy Susan (slow 360 orbit).
Mood: Powerful, coveted, dangerous.
Resolution: 720p (16:9)
Duration: 3 seconds
```

---

### 4. Примеры для Коммерциализации AI Проектов

#### Пример 9: SaaS Product Demo
```
Dashboard interface with real-time analytics scrolling. 
Graphs growing, numbers updating. 
The camera pushes in slowly to a specific chart showing revenue growth. 
Light reflects off monitor glass. 
Soft green glow from terminal indicates success.
Style: Cinematic corporate, modern, professional.
Camera: Dolly In + Focus Change to specific elements.
Mood: Growth, success, innovation.
Resolution: 1080p (16:9)
Duration: 4 seconds
```

#### Пример 10: AI Model Training Visualization
```
Lines of code flow rapidly across dark background, words glowing in neon green. 
Neural network nodes light up and connect. 
The camera crash zooms through layers of nodes, 
showing complexity and intelligence. 
Numbers and percentages update in real-time.
Style: Tech-forward, high-tech, Matrix-inspired.
Camera: Crash Zoom In/Out with multiple focus changes.
Mood: Powerful, intelligent, cutting-edge.
Resolution: 1080p (16:9)
Duration: 5 seconds
```

---

## Техники для видеопроизводства

### Техника 1: Многослойное движение (Compound Motion)

Комбинируйте несколько motion controls в одном промпте для сложного, профессионального вида:

```
A street dancer performs in crowded plaza. 
The camera performs multiple synchronized movements: 
first dolly in while orbiting around dancer (360 orbit + Dolly In), 
then tilts to Dutch angle to emphasize dynamic energy. 
Each spin and move is captured with handheld vibration for authenticity.
Camera: 360 Orbit + Dolly In + Dutch Angle + subtle Handheld shake
Style: Urban, energetic, documentary-style coverage
```

### Техника 2: Переходы между сценами (Seamless Transitions)

```
Scene 1: Офис в день – камера Dolly Out от сотрудника, 
раскрывая офисное пространство.

Scene 2: Тот же персонаж дома в ночи – камера Dolly In, 
фокусируясь на их лице. 
Создается ощущение плавного перехода.
```

### Техника 3: Синхронизация с аудио (Audio-Synced Motion)

Higgsfield Ultimate поддерживает синхронизацию видео с музыкой:

```
A rapper stands on stage, track beat drops. 
The camera snap-cuts forward on each bass hit (Rap Flex motion). 
Pulls back on verse, whips around on chorus. 
Every motion syncs perfectly with beat drops and rhythm changes.
```

### Техника 4: Контрастные движения (Contrast Dynamics)

Используйте контрастирующие движения для визуального интереса:

```
Wide aerial shot (Flying camera showing expansive landscape)
↓
Crash Zoom In на одного человека в поле
↓
Handheld shake as character reacts
↓
Slow Dolly Out revealing they're not alone
```

---

## Лучшие практики

### ✅ Что делать

1. **Будьте конкретны**
   - ❌ Плохо: "красивый закат"
   - ✅ Хорошо: "golden sunset bleeding across irradiated wasteland, dust devils swirling"

2. **Используйте кинематографический язык**
   - Слова: "tracking," "panning," "crane," "dolly," "zoom," "orbit," "low angle," "wide shot"

3. **Балансируйте детали и ясность**
   - Не перегружайте (max 2-3 motion controls вместе)
   - Фокусируйте на основных элементах

4. **Включайте движение и настроение**
   - Движение добавляет динамику
   - Слова настроения: "tense," "serene," "chaotic," "intimate," "epic"

5. **Используйте цвета и освещение**
   - "neon glow," "golden hour light," "harsh shadows," "soft diffuse light"

6. **Экспериментируйте с аспект-рейшо**
   - 16:9 для YouTube, Cinematic
   - 9:16 для TikTok, Reels, Shorts
   - 4:5 для Instagram Post
   - 2.35:1 для максимально кинематичного вида

### ❌ Чего избегать

1. **Слишком абстрактные описания**
   - ❌ "красивое видео с хорошей энергией"
   - ✅ "high-energy parkour sequence with dynamic aerial photography"

2. **Вводящие в заблуждение команды**
   - ❌ "make it look like movie" (размытое)
   - ✅ "cinematic 16:9 widescreen with warm color grading and film grain"

3. **Конфликтующие motion controls**
   - ❌ "Handheld + Robo Arm" (противоречат друг другу)
   - ✅ "Steady Robo Arm orbit" или "Handheld follow"

4. **Слишком много деталей**
   - ❌ Огромный промпт со 100 элементами
   - ✅ Сфокусированный промпт на 5-7 ключевых элементах

5. **Неправильная длина для контента**
   - ❌ 30-секундный промпт для 3-5 секундного видео
   - ✅ Адаптируйте масштаб к длительности

---

## Шпаргалка по стилям Higgsfield

| Стиль | Когда использовать | Пример описания |
|-------|-------------------|-----------------|
| **Cinematic** | Профессиональный контент | "High-resolution, polished visuals with balanced contrast and vivid colors" |
| **VHS** | Ретро, винтажные сцены | "Grain, noise, and color distortion like old video tapes" |
| **Super 8MM** | Домашняя кинопленка, ностальгия | "Grainy, warm-toned aesthetic of old film reels" |
| **Anamorphic** | Эпические, величественные сцены | "Wide dramatic aspect ratios with lens flares and subtle distortion" |
| **Abstract** | Экспериментальный контент | "Artistic and surreal, unconventional colors and shapes" |

---

## Быстрая ссылка: Структурный шаблон

Используйте этот шаблон как начало для всех промптов:

```
[ОСНОВНОЙ СУБЪЕКТ]: [живое описание персонажа/объекта]

[ДЕЙСТВИЕ]: [что происходит, динамика, движение]

[ОКРУЖЕНИЕ]: [локация, детали фона, архитектура]

[ОСВЕЩЕНИЕ]: [качество света, направление, цвета, время суток]

[КАМЕРА]: [specific motion control из списка выше]

[СТИЛЬ]: [Cinematic, VHS, Abstract, и т.д.]

[НАСТРОЕНИЕ]: [эмоциональный тон сцены]

[ТЕХНИЧЕСКИЕ ПАРАМЕТРЫ]: [Resolution, Aspect Ratio, Duration]
```

---

## Примеры готовых промптов для копирования

### Готовый промпт 1: Cyberpunk Drone Flight
```
Futuristic megacity at night with towering neon-lit skyscrapers and holographic advertisements. 
Flying cars weave through neon-soaked streets below. 
The camera executes aggressive FPV drone movements, 
diving through narrow passages between buildings, sharp turns around corners, 
weaving between aircraft with kinetic energy and speed. 
Neon reflections shimmer off buildings and street-level screens. 
Cyberpunk atmosphere with electric blues and magentas. 
Camera: FPV Drone with aggressive banking and turns. 
Resolution: 720p (16:9). Duration: 4 seconds.
```

### Готовый промпт 2: Emotional Character Study
```
Woman stands in abandoned train station, golden afternoon sunlight streaming through broken windows. 
Dust particles drift slowly through light beams. 
Her face shows quiet determination and weariness. 
The camera slowly performs a complete 360-degree orbit around her, 
starting at her profile, moving around to show her from all angles, 
emphasizing her solitude in the vast empty space. 
Graffitied walls and metal beams frame her isolation. 
Wind whistles through broken windows. 
Style: Cinematic drama with naturalistic lighting. 
Camera: Slow 360 Orbit. 
Mood: Solitude, resilience, quiet hope. 
Resolution: 720p (16:9). Duration: 5 seconds.
```

### Готовый промпт 3: Gaming/Mod Showcase
```
A heavily modified Fallout 4 character model stands in photorealistic post-apocalyptic wasteland. 
Custom armor gleams with metallic detail, weathered combat scars visible on surfaces. 
Sunset paints sky in orange and crimson. Ruins of old-world architecture frame the scene. 
The camera starts low behind the character, slowly craning upward to reveal the vast barren landscape. 
Dust devils swirl in distance. Wind blows through skeletal trees. 
Style: Photorealistic, gritty, post-apocalyptic with film grain overlay. 
Camera: Crane Up. 
Mood: Determined warrior, desolate hope. 
Resolution: 1080p (16:9). Duration: 4 seconds.
```

### Готовый промпт 4: Product Animation
```
Premium gaming mouse sits centered on clean black gaming desk with minimal setup. 
RGB lighting underneath desk casts soft blue glow. 
Mouse has intricate honeycomb design visible on matte black shell. 
Camera slowly orbits 360 degrees around the mouse at close range, 
showing every design detail, RGB accents, and texture variations. 
Professional studio lighting creates sharp reflections without harsh shadows. 
Style: Product photography, clean and minimalist. 
Camera: Lazy Susan (slow 360 orbit). 
Mood: Premium, desirable, high-tech. 
Resolution: 720p (9:16). Duration: 3 seconds.
```

---

## Заключение

С Higgsfield.ai Ultimate у вас есть доступ к:

✅ **50+ профессиональных motion controls**  
✅ **Неограниченные генерации** (1,500 кредитов/месяц)  
✅ **Без водяных знаков** для коммерческого использования  
✅ **Приоритетная обработка** для быстрых результатов  
✅ **4K генерация изображений** (Nano Banana Pro)  
✅ **Синхронизированный аудио** для видео  
✅ **Расширенное редактирование** и upscaling  

**Ключевой совет:** Начните с простых промптов, постепенно добавляя complexity. Экспериментируйте с разными motion controls, чтобы найти вашу уникальную визуальную подпись для видео-контента.

**Для вашего видеопроизводства:** Используйте Higgsfield для создания:
- Интро/Outro сцен для YouTube контента
- Переходов между сегментами
- Background визуалов для B-roll
- Демонстраций продуктов/проектов
- Сложных экшн-сцен (особенно для Fallout модов)
- Специальных эффектов и трансформаций

Удачи в создании контента! 🎬✨