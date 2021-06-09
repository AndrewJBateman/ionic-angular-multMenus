# :zap: Ionic Multiple Menus

* App that displays different menus for tabs 1 and 2.
* Tutorial code from [Simon Grimm of the Ionic Academy](https://www.youtube.com/user/saimon1924) see [:clap: Inspiration](#clap-inspiration) below
* **Note:** to open web links in a new window use: _ctrl+click on link_

![GitHub repo size](https://img.shields.io/github/repo-size/AndrewJBateman/ionic-angular-multMenus?style=plastic)
![GitHub pull requests](https://img.shields.io/github/issues-pr/AndrewJBateman/ionic-angular-multMenus?style=plastic)
![GitHub Repo stars](https://img.shields.io/github/stars/AndrewJBateman/ionic-angular-multMenus?style=plastic)
![GitHub last commit](https://img.shields.io/github/last-commit/AndrewJBateman/ionic-angular-multMenus?style=plastic)

## :page_facing_up: Table of contents

* [:zap: Ionic Multiple Menus](#zap-ionic-multiple-menus)
  * [:page_facing_up: Table of contents](#page_facing_up-table-of-contents)
  * [:books: General info](#books-general-info)
  * [:camera: Screenshots](#camera-screenshots)
  * [:signal_strength: Technologies](#signal_strength-technologies)
  * [:floppy_disk: Setup](#floppy_disk-setup)
  * [:computer: Code Examples](#computer-code-examples)
  * [:cool: Features](#cool-features)
  * [:clipboard: Status & To-do list](#clipboard-status--to-do-list)
  * [:clap: Inspiration](#clap-inspiration)
  * [:file_folder: License](#file_folder-license)
  * [:envelope: Contact](#envelope-contact)

## :books: General info

* Tab1 and Tab2 both contain ion-menus and a side-bar with routing to 2 pages.

## :camera: Screenshots

![Ionic page](./img/menu1.png)
![Ionic page](./img/menu2.png)

## :signal_strength: Technologies

* [Ionic v5](https://ionicframework.com/)
* [Angular v12](https://angular.io/)
* [Ionic/angular v5](https://www.npmjs.com/package/@ionic/angular)

## :floppy_disk: Setup

* Run `npm i` to install dependencies
* To start the server on _localhost://8100_ type: 'ionic serve'

## :computer: Code Examples

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

## :cool: Features

* Uses a `panelEnabled` boolean value to control menu disabling.

## :clipboard: Status & To-do list

* Status: Working. Updated june 2021.
* To-do: Nothing.

## :clap: Inspiration

* [Simon Grimm, Ionic Academy Tutorial: Multiple Side Menus With Ionic Tab Bar](https://www.youtube.com/watch?v=4VYC725VMNA)

## :file_folder: License

* This project is licensed under the terms of the MIT license.

## :envelope: Contact

* Repo created by [ABateman](https://github.com/AndrewJBateman), email: gomezbateman@yahoo.com
