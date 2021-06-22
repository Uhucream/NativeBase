# <img src="./img/header1.png" alt="Nativebase Logo"> 

[![Financial Contributors on Open Collective](https://opencollective.com/NativeBase/all/badge.svg?label=financial+contributors)](https://opencollective.com/NativeBase) [![](http://slack.nativebase.io/badge.svg)](http://slack.nativebase.io/) [![Build Status](https://travis-ci.org/GeekyAnts/NativeBase.svg?branch=master)](https://travis-ci.org/GeekyAnts/NativeBase) [![npm version](https://badge.fury.io/js/native-base.svg)](https://badge.fury.io/js/native-base) [![npm downloads](https://img.shields.io/npm/dt/native-base.svg)](https://npm-stat.com/charts.html?package=native-base&from=2016-04-01&to=2018-02-17)

A complete component library for React Native Ecosystem

- **Accessible** : Maximise app usage with our accessible design.
- **Responsive** : Create responsive apps with ease from the get-go.
- **Themeable** : Customise your app theme and component styles.
- **Consistent** : Make accurate predictions for web, Android & iOS.

## Documentation
You can find the complete documentation [here](https://docs.nativebase.io/).

## Table of Content

1. [Introduction](#1-introduction)
2. [Motivation](#2-motivation)
3. [Features](#3-features)
4. [Dependencies](#4-dependencies)
5. [Installation & Setup](#5-installation-&-setup)
6. [Components](#6-components)
7. [Examples](#7-examples)
8. [KitchenSink App](#8-kitchensink-app)
9. [Tech Stack](#9-tech-stack)
10. [Compatible Versions](#10-compatible-versions)
11. [Contributors](#11-contributors)
12. [Changelog](#12-changelog)
13. [Community](#13-community)
14. [License](#14-license)


## 1. Introduction?
[NativeBase](https://nativebase.github.io/) is a mobile-first, component library for React & React Native. Version 3.0 ships with complete ARIA integration, support for utility props and nearly 40 components that are consistent across Android, iOS and Web. Fast-track your dev process with NativeBase 3.0.

**Recommended by [Awesome React Native](https://github.com/jondot/awesome-react-native)**

NativeBase was added to the list of Frameworks of Awesome React Native and it is used by numerous React lovers across the world.
## 2. Motivation
Building with React Native from scratch is a tedious process with multiple steps such as adding styling, interactions, state management, responsiveness, accessibility, etc. We wanted to build and ship accessible, high-quality apps quickly.
<br />

Our inspirations include Material UI, Chakra UI, Ant Design, Braid Design System, Bootstrap, TailwindCSS & Flutter.

## 3. Features

### **Out of the Box Accessibility**

Integrated with React ARIA and React Native ARIA, which provides React hooks. This enables you to build accessible design systems in no time.

<img src="./img/feature.png" alt="Out of the box accessibility"> 

### **Supporting Utility Props**

Powered by [Styled System](https://styled-system.com) so you can rapidly build custom UI components with constraint-based utility style props.

### **Rich Component Library**

NativeBase offers around 40 components so you can build seamlessly. It includes button, checkbox, flex, stack and more.

### **Highly Themeable**

Themeability is one of the core elements of NativeBase. You can customise your app theme and component styles to your heart's content.

<img src="./img/theme.png" alt="Nativebase Logo"> 

### **Available for Both Mobile and Web**

NativeBase 3.0 is powered by React Native Web so you can build consistent UIs across Web, Android and iOS.

### **Responsiveness Made Easy**

Instead of manually adding responsiveness, NativeBase 3.0 allows you to provide object and array values to add responsive styles.

### **Now with** **Dark Mode**

Building apps with a dark mode setting just got a whole lot easier. NativeBase is now optimised for light and dark modes.

## 4. Dependencies

React Native, Expo

## 5. Installation & Setup

To start using NativeBase components in your native apps, create a new React Native project. [Expo](https://docs.expo.io/get-started/installation/) is a great starting point so let's set it up, install NativeBase using yarn/npm and add all the peer dependencies. To get `NativeBase` running onto your native apps, install it using `npm` or `yarn`.

### Setup with React Native

```bash
react-native init AwesomeNativeBase
cd AwesomeNativeBase
```

*Install **NativeBase***

```bash
# using yarn
yarn add native-base@next react-native-svg styled-components styled-system react-native-safe-area-context
```

```bash
# using npm
npm install native-base@next react-native-svg styled-components styled-system react-native-safe-area-context
```

*Run pod install*

```bash
cd ios/
pod install
```

You've successfully setup [NativeBase](https://nativebase.io/) with your [React Native](https://reactnative.dev/) app. Your React Native app is ready to run on iOS and Android devices.

### Setup with Expo

Expo helps you to create universal (iOS, Android and Web) React Native apps with no build configuration.

*Install **NativeBase***

```bash
# using yarn
yarn add native-base@next styled-components styled-system
expo install react-native-svg
expo install react-native-safe-area-context
```

```bash
# using npm
npm install native-base@next styled-components styled-system
expo install react-native-svg
expo install react-native-safe-area-context
```

### Setup for Next.js with Expo for Web

```bash
# using yarn
yarn add native-base@next react-native-svg @expo/vector-icons styled-components styled-system
```

```bash
# using npm
npm i native-base@next react-native-svg @expo/vector-icons styled-components styled-system
```

By default Next.js doesn't support static assets like an Expo project. Because this is the intended functionality of Next.js, @expo/next-adapter doesn't add font support by default. If you want to use libraries like expo-font, @expo/vector-icons, you'll need to change a few things.

```bash
yarn add next-fonts
```
Wrap the font method with the Expo method in your next.config.js:

```js
const { withExpo } = require('@expo/next-adapter');
const withFonts = require('next-fonts');

module.exports = withExpo(
  withFonts({
    projectRoot: __dirname,
  })
);
```
The order is important because Expo can mix in the location of vector icons to the existing font loader.Now restart your project and you should be able to load fonts!

## 6. Components

NativeBase 3.0 is a rich component library with nearly 40 components.
  
- [**Layout**](https://docs.nativebase.io/box)   
- [**Forms**](https://docs.nativebase.io/button)
- [**Data Display**](https://docs.nativebase.io/badge)
- [**Feedback**](https://docs.nativebase.io/alert)
- [**Typography**](https://docs.nativebase.io/text)
- [**Overlay** ](https://docs.nativebase.io/alertDialog)
- [**Disclosure**](https://docs.nativebase.io/actionSheet)
- [**Media & Icons**](https://docs.nativebase.io/avatar)
- [**Transition**](https://docs.nativebase.io/presence-transition)
- [**Other**](https://docs.nativebase.io/FAB)
    

## 7. Examples

Check out the Login Screen example [here](https://docs.nativebase.io/todo-example)


## 8. KitchenSink App

Kitchen Sink is a comprehensive demo app showcasing all the NativeBase components in action. It includes buttons, forms, icons, etc.

<table>
  <tr>
    <td style="border:0px;"><img src="./img/kitchensink.gif" width="50%" style="margin-right:50px" alt="Kitchensink App gif"></td>
    <td style="border:0px;"><img src="./img/scan_kitchensink.png" width="50%" style="align-self: center;" alt="Kitchensink App QR code"></td>
  </tr>
</table>


## 9. Tech Stack

JavaScript, React Native, Styled System

## 10. Compatible Versions

| NativeBase          		    | React Native   	            |
| --------------------------------|-------------------------|
| v0.1.1			                    | v0.22 to v0.23          |					 
| v0.2.0 to v0.3.1	  		        |	v0.24 to v0.25			 	  |
| v0.4.6 to v0.4.9	  		        |	v0.26.0 - v0.27.1			 	|
| v0.5.0 to v0.5.15	  		        |	v0.26.0 - v0.37.0			 	|
| v0.5.16 to v0.5.20	  	        | v0.38.0 - v0.39.0				|
| v2.0.0-alpha1 to v2.1.3	        |	v0.38.0 to v0.43.0			|	
| v2.1.4 to v2.1.5	  		        |	v0.44.0 to v0.45.0			|
| v2.2.0			  		              | v0.44.0 to v0.45.0			|
| v2.2.1			  		              |	v0.46.0 and above				|
| v2.3.0 to 2.6.1	  		          | v0.46.0 and above (does not support React 16.0.0-alpha.13) |
| v2.7.0			  		              |	v0.56.0 and above			 	|
| v3.0.0-next.36 to v3.0.0-next-41 | v0.63.0 and above      | 

## 11. Contributors

### Code Contributors

This project exists thanks to all the people who contribute. [[Contribute](CONTRIBUTING.md)].
<a href="https://github.com/GeekyAnts/NativeBase/graphs/contributors"><img src="https://opencollective.com/NativeBase/contributors.svg?width=890&button=false" /></a>

### Financial Contributors

Become a financial contributor and help us sustain our community. [[Contribute](https://opencollective.com/NativeBase/contribute)]

#### Individuals

<a href="https://opencollective.com/NativeBase"><img src="https://opencollective.com/NativeBase/individuals.svg?width=890"></a>

#### Organizations

Support this project with your organization. Your logo will show up here with a link to your website. [[Contribute](https://opencollective.com/NativeBase/contribute)]

<a href="https://opencollective.com/NativeBase/organization/0/website"><img src="https://opencollective.com/NativeBase/organization/0/avatar.svg"></a>
<a href="https://opencollective.com/NativeBase/organization/1/website"><img src="https://opencollective.com/NativeBase/organization/1/avatar.svg"></a>
<a href="https://opencollective.com/NativeBase/organization/2/website"><img src="https://opencollective.com/NativeBase/organization/2/avatar.svg"></a>
<a href="https://opencollective.com/NativeBase/organization/3/website"><img src="https://opencollective.com/NativeBase/organization/3/avatar.svg"></a>
<a href="https://opencollective.com/NativeBase/organization/4/website"><img src="https://opencollective.com/NativeBase/organization/4/avatar.svg"></a>
<a href="https://opencollective.com/NativeBase/organization/5/website"><img src="https://opencollective.com/NativeBase/organization/5/avatar.svg"></a>
<a href="https://opencollective.com/NativeBase/organization/6/website"><img src="https://opencollective.com/NativeBase/organization/6/avatar.svg"></a>
<a href="https://opencollective.com/NativeBase/organization/7/website"><img src="https://opencollective.com/NativeBase/organization/7/avatar.svg"></a>
<a href="https://opencollective.com/NativeBase/organization/8/website"><img src="https://opencollective.com/NativeBase/organization/8/avatar.svg"></a>
<a href="https://opencollective.com/NativeBase/organization/9/website"><img src="https://opencollective.com/NativeBase/organization/9/avatar.svg"></a>

## 12. Changelog

## 13. Community
- [Facebook](https://www.facebook.com/nativebaseio)
- [Twitter](https://twitter.com/nativebaseio)
- [Discord](https://discord.com/invite/TSgCw2UPmb)
- [Stackoverflow](https://stackoverflow.com/questions/tagged/native-base)
- [Medium](https://blog.nativebase.io/)
- [YouTube](https://www.youtube.com/channel/UCoL_iTwpY07vDs91974z3xA/about)
## 14. License
Licensed under the MIT License, Copyright © 2020 GeekyAnts. See [LICENSE](https://github.com/GeekyAnts/NativeBase/blob/master/LICENSE) for more information.
