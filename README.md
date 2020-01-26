# Ionic Multiple Menus

App that displays different menus for tabs 1 and 2.

## Table of contents

* [General info](#general-info)
* [Screenshots](#screenshots)
* [Technologies](#technologies)
* [Setup](#setup)
* [Features](#features)
* [Status](#status)
* [Inspiration](#inspiration)
* [Contact](#contact)

## General info

* Tab1 and Tab2 both contain ion-menus and a side-bar with routing to 2 pages.

## Screenshots

![Ionic page](./img/menu1.png)
![Ionic page](./img/menu2.png)


## Technologies

* [Ionic v5.0.0](https://ionicframework.com/)
* [Angular v8.1.2](https://angular.io/)
* [Ionic/angular v4.7.1](https://www.npmjs.com/package/@ionic/angular)

## Setup

* To start the server on _localhost://8100_ type: 'ionic serve'

## Code Examples

* Tab1 page code to show first (of two) menus using the [Ionic MenuController provider](https://ionicframework.com/docs/v3/api/components/app/MenuController/).

```typescript
export class Tab1Page {
  panelEnabled = true;
  constructor(private menuController: MenuController) {}

  ionViewWillEnter() {
    this.panelEnabled = true;
    this.menuController.enable(true, 'first');
  }

  ionViewWillLeave() {
    this.panelEnabled = false;
  }
```

## Features

* Uses a `panelEnabled` boolean value to control menu disabling. 

## Status & To-do list

* Status: Working

* To-do: nothing. Could use this multiple menu in other Ionic apps.

## Inspiration

* [Simon Grimm, Ionic Academy Tutorial: Multiple Side Menus With Ionic Tab Bar](https://www.youtube.com/watch?v=4VYC725VMNA)

## Contact

Repo created by [ABateman](https://www.andrewbateman.org) - feel free to contact me!