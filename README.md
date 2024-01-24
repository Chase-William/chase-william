## Hello, My Name is Chase 👋 
I'm a 2023 graduate of <a href="https://www.rit.edu/">Rochester Institute of Technology</a> with a bachelor's degree in <a href="https://www.rit.edu/study/web-and-mobile-computing-bs">Web & Mobile Computing</a> and a minor in Psychology.

#### Hobbies
- Coding *(Mit meine Kaffee!)*
- Exploring different technologies and spaces through development of personal projects 🌱
- Weight Lifting 💪 / Calisthenics
- Currently embarked on reading the Wheel of Time series by Robert Jordan *(14 books.. its long)*
- Playing my guitars 🎸
- Memorizing power quotes

#### Other Interest or Things About Me
- I have a personal website: [chase-william.net](https://chase-william.net)
- Currently, my favorite technologies include: [.NET](https://dotnet.microsoft.com/), [C#](https://docs.microsoft.com/en-us/dotnet/csharp/), [TypeScript](https://www.typescriptlang.org/), [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript), [Auto Hotkey](https://www.autohotkey.com/), [VS Code](https://code.visualstudio.com/), [Markdown](https://en.wikipedia.org/wiki/Markdown), [Github](https://github.com/) 🧪
- Am hard of hearing
- ASL proficient 🤌
- Studied German during high school on own accord. Also took Deutsch ein *(1)* at RIT, therefore know the basics.
- Due to playing tank & plane games in my youth, I have amounted a knowledge base of WW1 & WW2 tanks & planes. Favorite tanks include: [IS-3](https://en.wikipedia.org/wiki/IS-3), [IS-7](https://en.wikipedia.org/wiki/IS-7), [Panther A](https://en.wikipedia.org/wiki/Panther_tank), [Tiger I](https://en.wikipedia.org/wiki/Tiger_I), [Jagdpanzer IV](https://en.wikipedia.org/wiki/Jagdpanzer_IV), [T29 *With it's Ears* (rangefinders)](https://en.wikipedia.org/wiki/T29_Heavy_Tank), [T34](https://en.wikipedia.org/wiki/T34_Heavy_Tank), [The Jumbo *(m4a3e2)*](https://tanks-encyclopedia.com/ww2/us/m4a3e2-jumbo-assault-tank)

> About my projects: Whether the project was finished or not, I see a win. These experiences only leave me a better developer than when I started.

## Notable Projects:

### DotDocs

Generate easy add hoc docs from your C# codebase in markdown format. Read more [here](https://github.com/Chase-William/DotDocs).

![DotDocs_how_it_works](https://github.com/Chase-William/chase-william/assets/46757278/fcbe5d31-e5b8-4ff0-8b0e-e646cdae8724)

### Tribe Logger

*Tribe Logger* aims to provide members with updates/notification about tribe log information when in-game events occur. The updates/notifications are provided via a `Discord Bot`. For the client application, I am using `Electron` with my own native node addons to basically get text from a window using [`OCR`](https://en.wikipedia.org/wiki/Optical_character_recognition).

> To get text from a window, I first aquire bitmaps from a window on command using it's [Device Context](https://docs.microsoft.com/en-us/windows/win32/gdi/device-contexts). The bitmap is then either piped all the way up to the `TypeScript` / `JavaScript` to be displayed in a canvas *(for previewing)*, or given to [tesseract](https://github.com/tesseract-ocr/tesseract) *(building from source using [vcpkg](https://github.com/microsoft/vcpkg))* inside the native `C++` addon to decipher text and return it to the caller.

In the image below you can see it capturing a bitmap from the *ARK: Survival Evolved* window and then displaying it in the `Electron` app window. The green box is the area the user can crop for tesseract to scan for text. *(testing right now)*

![Tribe-Logger](resources/tribe-logger/testing.png)

I ported the project to use this [template](https://github.com/electron-react-boilerplate/electron-react-boilerplate) to help speed up `React` integration.

### Game Of Life

This project was created for [ICS](https://www.rit.edu/ntid/ics) department and moreover the [SVP](https://www.rit.edu/ntid/svp) group of 2021. It is based off the [*Game Of Life*](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life) and is available on:
- Console *(.NET Core)*
- Desktop *(WPF .NET Core)*
- Mobile *(Android using Xamarin)*

> Note: The console also accepts input for *Rows*, *Columns*, and *Cycle Time*, but in the provided screenshot you cannot see it because it has been cleared away...*

![Game Of Life Console, Desktop, & Mobile](resources/game-of-life/game_of_life_all.png)

I attended the event and assisted new students with building their own apps from this repo. Checkout the [repo](https://github.com/MAD-NTID/GameOfLife) if you want to see more or download it for youself.

### Lil Widgets

[*Lil Widgets*](https://github.com/Chase-William/LilWidgets) is a library that provides progress & loading widgets to `Xamarin.Forms`. The motive behind this project was I wanted to learn more about animations and how to create them. Therefore this project depends heavily on `SkiaSharp` and its various public packages.

I created the widgets from scratch using `SkiaSharp` and it's `SKCanvasView` type. I learned about creating my own `Delta-Time` implementation *(used it before in `Unity`)* and how to implement better animation update routines *(moving away from frame rate based update to time based)*. I never felt my own implementations were smooth enough so I ended up coupling my animations to the built-in [Animation](https://docs.microsoft.com/en-us/dotnet/api/xamarin.forms.animation?view=xamarin-forms) class *(uses native animation utilities)*.

> This project's underlying structure is based off [Microcharts](https://github.com/microcharts-dotnet/Microcharts), except *Lil Widgets* repo is coupled to `Xamarin.Forms` as I previously mentioned.

| Progress Widget | Progress Breakdown | Loading Widget |
| :---: | :---: | :---: |
| ![Home Page](resources/lil-widgets/progress_widget.jpg) | ![Quiz Page](resources/lil-widgets/progress_widget_breakdown.jpg) | ![Quiz Page](resources/lil-widgets/loading_widget.jpg) |

Checkout more about this project at its [repo](https://github.com/Chase-William/LilWidgets)...

### Baby Fingers

The app, *Baby Fingers* uses `Xamarin.Forms` to provide both `Android` & `iOS` packages. It is available on both `Google Play` and the `Apple App Store`. The app provides various topics that have lessons within them with quizzes to test your memory once you're ready!

|  |  |  |
| :---: | :----: | :---: |
| ![Home Page](resources/baby-fingers/home_page.png) | ![Quiz Page](resources/baby-fingers/taking_quiz_page.png) | ![Quiz Attempts](resources/baby-fingers/quiz_attempts_page.png) |

The *Baby Fingers* repo is not currently available to the public to protect the client.
