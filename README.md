### Hello, I'm Chase 👋
I'm a 4rd year Web and Mobile Computing undergraduate at <a href="https://www.rit.edu/">Rochester Institute of Technology</a>.

- 🌱 Currently learning & building an [electron](https://www.electronjs.org/) app with [React](https://reactjs.org/) which includes my very own [native node addon](https://nodejs.org/api/addons.html) using [nan](https://github.com/nodejs/nan)
- 🧪 Favorite technologies: [.NET](https://dotnet.microsoft.com/), [GoLang](https://golang.org/), [SkiaSharp](https://docs.microsoft.com/en-us/xamarin/xamarin-forms/user-interface/graphics/skiasharp/), [ML.NET](https://dotnet.microsoft.com/apps/machinelearning-ai/ml-dotnet)
- 🔭 Currently employed as a Teaching Assistant and as the Lead Tutor of the <a href="https://www.rit.edu/ntid/ics">ICS Department</a>.

## Projects

### Tribe Logger
Tribe Logger aims to provide members with updates about tribe log information when in-game events occur. This is where native-node addons come in as I am using my own to get bitmaps from a window on command using it's [Device Context](https://docs.microsoft.com/en-us/windows/win32/gdi/device-contexts). This is then either piped all the way up to JS and displayed in a canvas or given to [tesseract](https://github.com/tesseract-ocr/tesseract) *(building from source using [vcpkg](https://github.com/microsoft/vcpkg))*.

In the image below you can see it capturing a bitmap from the `ARK: Survival Evolved` window and then displaying it in the `Electron` app window. The green box is the area the user can `crop` for tesseract to scan for text.
![Tribe-Logger](resources/tribe-logger/testing.png)

Recently I ported the project to use this [template](https://github.com/electron-react-boilerplate/electron-react-boilerplate) to help speed up `React` integration.

#### Remaining:
 - Finish Front-End / Packaging *using [webpack](https://webpack.js.org/) | [babel](https://babeljs.io/)*
 - Build a `Rest API` coupled to a `DBMS` and it's database *(client authentication needed | probs gonna go [mySQL](https://www.mysql.com/) 8.0)*
 - Build the `Discord Bot` *(using [GoLang](https://golang.org/) & [discordGo](https://github.com/bwmarrin/discordgo))*

Tribe Logger is a electron app that is being build with React as it's front-end JS framework.

This repo is currently under active development and is private because of possible monetization once finished. 

### Game Of Life
This project was created for [ICS](https://www.rit.edu/ntid/ics) department and moreover the [SVP](https://www.rit.edu/ntid/svp) group of 2021. It is based off the [Game Of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life) and is available on:
- Console *(.NET Core)*
- Desktop *(WPF .NET Core)*
- Mobile *(Android using Xamarin)*

// Add Images Here

I attended the event and assisted new students with building their own apps from this repo. Checkout the [repo](https://github.com/MAD-NTID/GameOfLife) if you want to see more or download it for youself.

### Baby Fingers

The app Baby Fingers uses Xamarin.Forms to provide both Android & iOS packages. It is available on both Google Play and the Apple App Store.

|  |  |  |
| :---: | :----: | :---: |
| ![Home Page](resources/baby-fingers/home_page.png) | ![Quiz Page](resources/baby-fingers/taking_quiz_page.png) | ![Quiz Attempts](resources/baby-fingers/quiz_attempts_page.png) |
