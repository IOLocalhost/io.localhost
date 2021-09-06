# io.localhost - lib

Library to build javascript scripts for the bloble.io game.

Script development for bloble.io

## install script
```js
    const ioSection = $("<section />", {
        id: 'ioSection',
        class: 'ioSection'
    })
 
    const ioLib = $("<script />", {// code
        src: 'https://io-localhost.vercel.app/assets/javascript/lib/file.lib.js'
    })
 
    $("#darkener").append(ioSection)
    $("#ioSection").append(ioLib)
 
 
$("#enterGameButton").click(() => {
  // you code here
})
```

### your code here
The code you will assemble must be inside, because outside there are only the section creation code and the lib code link for the bloble to read.
> Our bookstore using modern javascript is object-oriented javascript.
> 
> recommendation do not mess out.

# Use

### Create a menu with a single value.

**Following the Steps**
- [ ] Create a constant with any name.
- [ ] Using the constant to build the menu.
- [ ] Creating the Button and function ID.
- [ ] Create function.

### Stage (1)
Create a constant with any name.
```js
const menuHello_example = new MenuBuild()
```
- [x] Create a constant with any name. ( Done )


### Stage (2) 
Using the constant to build the menu.
```js
menuHello_example.mount()
```
- [x] Create a constant with any name. ( Done )
- [x] Using the constant to build the menu. ( Done )


### Stage (3)
Creating the Button and function ID.
```js
menuHello_example.addItem("Hello World","hello")
```
- [x] Create a constant with any name. ( Done )
- [x] Using the constant to build the menu. ( Done )
- [x] Creating the Button and function ID. ( Done )

### Stage (4)
Create function.
```js
$("#hello").click(() => { alert('Hello World') })
```
- [x] Create a constant with any name. ( Done )
- [x] Using the constant to build the menu. ( Done )
- [x] Creating the Button and function ID. ( Done )
- [x] Create function. ( Done )

### Result

![result](https://media.discordapp.net/attachments/857742055442874408/884262946409156608/Captura_de_tela_2021-09-05_23-24-43.png)

> Code
> ```js
> const menuHello_example = new MenuBuild()
> menuHello_example.mount()
> menuHello_example.addItem("Hello World", "hello")
> $("#hello").click(() => { alert('Hello World')})

***

### Creating themes
**Following the Steps**
- [ ] Create a constant with any name.
- [ ] Adding to the colors in the object.
- [ ] Applying the theme.

### Stage (1)
Create a constant with any name.
```js
const example = new Theme()
```
- [x] Create a constant with any name. ( Done )

### Stage (2)
Adding to the colors in the object.
```js
// There are four color values, they follow the game order (backgroundColor, outerColor, indicatorColor, redColor)
const darkTheme_exemple = new Theme( "rgb(10, 10, 10)" , "rgb(20, 20, 20)" , "#222" , "rgba(200, 0, 0, 0.5)")
```
- [x] Create a constant with any name. ( Done )
- [x] Adding to the colors in the object. ( Done )

### Stage (3)
 Applying the theme.
```js
darkTheme_exemple.applyTheme()
```
- [x] Create a constant with any name. ( Done )
- [x] Adding to the colors in the object. ( Done )
- [x] Applying the theme. ( Done )

### Result

![result](https://media.discordapp.net/attachments/857742055442874408/884266982973767710/Captura_de_tela_2021-09-05_23-40-51.png)

> Code
> ```js
> const darkTheme_exemple = new Theme( "rgb(10, 10, 10)" , "rgb(20, 20, 20)" , "#222" , "rgba(200, 0, 0, 0.5)")
> darkTheme_exemple.applyTheme()

***

### Creating Item Upgrade
**Following the Steps**
- [ ] Create a constant with any name. 
- [ ] Add item name inside object.
- [ ] Creating Menu and Upgrade Button.
- [ ] Creating Function.
- [ ] Update Item. 

### Stage (1)
Create a constant with any name. 
```js
const exampleItemUpgrade = new Item("")
```
- [x] Create a constant with any name. ( Done )

### Stage (2)
add item name inside object
```js
const itemUpgrade_example = new Item("gen")// upgrate power
```
- [x] Create a constant with any name. ( Done )
- [x] add item name inside object. ( Done )

### Stage (3)
Creating Menu and Upgrade Button.
```js
const menu_example = new MenuBuild()
menu_example.mount()
menu_example.addItem("Power Plants", "genUpdate")
```
- [x] Create a constant with any name. ( Done )
- [x] add item name inside object. ( Done )
- [x] Creating Menu and Upgrade Button. ( Done )

### Stage (4)
Creating Function.
```js
$("#genUpdate").click(() => {
//code here
})
```
- [x] Create a constant with any name. ( Done )
- [x] add item name inside object. ( Done )
- [x] Creating Menu and Upgrade Button. ( Done )
- [x] Creating Function. ( Done )

### Stage (5)
Update Item.
```js
itemUpgrade_example.upgrade()
```

### Result 
![result](https://media.discordapp.net/attachments/857742055442874408/884272002259644446/Captura_de_tela_2021-09-06_00-00-28.png)

### (click)

![result](https://media.discordapp.net/attachments/857742055442874408/884271991832600666/Captura_de_tela_2021-09-06_00-00-46.png)

> Code
> ```js
> const itemUpgrade_example = new Item("gen")// upgrate power
> const menu_example = new MenuBuild()
> menu_example.mount()
> menu_example.addItem("Power Plants", "genUpdate")
> $("#genUpdate").click(() => {
>   itemUpgrade_example.upgrade()
> })
> ```

***
### Creating a complete menu
* ***In our menu will include***
    * Upgrade Walls
    * Upgrade Generator.
    * Upgrade All Turrets.
    * Themes.


**Following the Steps**
- [ ] Create a constant with any name.
- [ ] Defining update items.
- [ ] Defining Themes.
- [ ] Creating the menu with buttons.
- [ ] defining the functions

### Stage (1/2)
Create a constant with any name.
```js
const boulders = new Item("boulder")
const spikes = new Item("spikes")
const micro = new Item("micro")
const power = new Item("power")

const rapid = new Item("rapidTurret")
const gatlin = new Item("gatlinTurret")
const ranged = new Item("rangedTurret")
const spotter = new Item("spotterTurret")
const anti = new Item("Antitank")
const semi = new Item("semiAuto")
```
- [x] Create a constant with any name. ( Done )
- [x] Defining update items. ( Done )

### Stage (3)
Defining Themes.
```js
    const whiteTheme = new Theme("#ebebeb", "#d6d6d6", "rgba(0,0,0,0.08)", "rgba(255, 0, 0, 0.1)")
    const darkTheme = new Theme( "rgb(10, 10, 10)" , "rgb(20, 20, 20)" , "#222" , "rgba(200, 0, 0, 0.5)")
    const daculaTheme = new Theme("#1e1a30", "#454545", "#bc04bf", "#04bf23")
    const vueTheme = new Theme("#35495E", "#37587a", "rgba(196, 196, 196, 0.5)", "#41B883")
    const vscodeTheme = new Theme("#242220", "#383533", "#17692b", "#009dff")
    const githubWhiteTheme = new Theme("#ebebeb", "#8a8a88", "#8f000e", "#00158f")
    const githubDarkTheme = new Theme("#0d1117", "#263142", "#7d0b7b", "#0b3b7d")
```
- [x] Create a constant with any name. ( Done )
- [x] Defining update items. ( Done )
- [x] Defining Themes. ( DOne )

### Stage (4) 
Creating the menu with buttons.
```js
const menu = new MenuBuild()
menu.mount()
menu.addItem("Boulders","boulder")
menu.addItem("Spikes","spike")
menu.addItem("Micro-Gen","micro")
menu.nextLine()// line-break
menu.addItem("Rapid Turret","rapid")
menu.addItem("Gatlin Turret","gatlin")
menu.addItem("Ranged Turret","ranged")
menu.addItem("Spotter Turret","sppoter")
menu.nextLine()// line-break
menu.addItem("Anti-Tank","anti")
menu.addItem("Semi Auto","semi")
menu.nextLine()// line-break
menu.addItem("White", "whiteTheme")
menu.addItem("Dark", "darkTheme")
menu.addItem("Dracula", "daculaTheme")
menu.addItem("Vue", "vueTheme")
menu.addItem("Visual Studio Code", "vscodeTheme")
menu.addItem("Github White", "githubWhiteTheme")
menu.addItem("Github Dark", "githubDarkTheme")
```
- [x] Create a constant with any name. ( Done )
- [x] Defining update items. ( Done )
- [x] Defining Themes. ( Done )
- [x] Creating the menu with buttons. ( Done )


### Stage (5)
defining the functions

```js
$("#boulder").click(() => { 
    boulders.upgrade()
})

$("#spike").click(() => { 
    spikes.upgrade()
})

$("#micro").click(() => { 
    micro.upgrade()
})

$("#rapid").click(() => { 
    rapid.upgrade()
})

$("#gatlin").click(() => { 
    gatlin.upgrade()
})

$("#sppoter").click(() => { 
    sppoter.upgrade()
})

$("#anti").click(() => {
    anti.upgrade()
})

$("#semi").click(() => {
    semi.upgrade()
})

$("#whiteTheme").click(() => {
    whiteTheme.applyTheme() 
})

$("#darkTheme").click(() => { 
    darkTheme.applyTheme()
})

$("#daculaTheme").click(() => { 
    daculaTheme.applyTheme() 
})

$("#vueTheme").click(() => { 
    vueTheme.applyTheme() 
})

$("#vscodeTheme").click(() => { 
    vscodeTheme.applyTheme() 
})

$("#githubWhiteTheme").click(() => { 
    githubWhiteTheme.applyTheme() 
})

$("#githubDarkTheme").click(() => { 
    githubDarkTheme.applyTheme() 
})
```
- [x] Create a constant with any name. ( Done )
- [x] Defining update items. ( Done )
- [x] Defining Themes. ( Done )
- [x] Creating the menu with buttons. ( Done )
- [x] Defining the functions. ( Done )

### Result

![result](https://media.discordapp.net/attachments/857742055442874408/884412048044351538/Captura_de_tela_2021-09-06_09-16-57.png)

> Code
> ```js
> 
> const boulders = new Item("boulder")
> const spikes = new Item("spikes")
> const micro = new Item("micro")
> const power = new Item("power")
>
> const rapid = new Item("rapidTurret")
> const gatlin = new Item("gatlinTurret")
> const ranged = new Item("rangedTurret")
> const spotter = new Item("spotterTurret")
> const anti = new Item("Antitank")
> const semi = new Item("semiAuto")
> 
> const whiteTheme = new Theme("#ebebeb", "#d6d6d6", "rgba(0,0,0,0.08)", "rgba(255, 0, 0, 0.1)")
> const darkTheme = new Theme( "rgb(10, 10, 10)" , "rgb(20, 20, 20)" , "#222" , "rgba(200, 0, 0, 0.5)")
> const daculaTheme = new Theme("#1e1a30", "#454545", "#bc04bf", "#04bf23")
> const vueTheme = new Theme("#35495E", "#37587a", "rgba(196, 196, 196, 0.5)", "#41B883")
> const vscodeTheme = new Theme("#242220", "#383533", "#17692b", "#009dff")
> const githubWhiteTheme = new Theme("#ebebeb", "#8a8a88", "#8f000e", "#00158f")
> const githubDarkTheme = new Theme("#0d1117", "#263142", "#7d0b7b", "#0b3b7d")
>
> const menu = new MenuBuild()
> menu.mount()
> menu.addItem("Boulders","boulder")
> menu.addItem("Spikes","spike")
> menu.addItem("Micro-Gen","micro")
> menu.nextLine()// line-break
> menu.addItem("Rapid Turret","rapid")
> menu.addItem("Gatlin Turret","gatlin")
> menu.addItem("Ranged Turret","ranged")
> menu.addItem("Spotter Turret","sppoter")
> menu.nextLine()// line-break
> menu.addItem("Anti-Tank","anti")
> menu.addItem("Semi Auto","semi")
> menu.nextLine()// line-break
> menu.addItem("White", "whiteTheme")
> menu.addItem("Dark", "darkTheme")
> menu.addItem("Dracula", "daculaTheme")
> menu.addItem("Vue", "vueTheme")
> menu.addItem("Visual Studio Code", "vscodeTheme")
> menu.addItem("Github White", "githubWhiteTheme")
> menu.addItem("Github Dark", "githubDarkTheme")
> 
> $("#boulder").click(() => {
>     boulders.upgrade()
> })
> 
> $("#spike").click(() => {
>     spikes.upgrade()
> })
> 
> $("#micro").click(() => {
>     micro.upgrade()
> })
> 
> $("#rapid").click(() => {
>     rapid.upgrade()
> })
> 
> $("#gatlin").click(() => {
>    gatlin.upgrade()
> })
>
> $("#sppoter").click(() => {
>    sppoter.upgrade()
> })
>
> $("#anti").click(() => {
>    anti.upgrade()
> })
>
> $("#semi").click(() => {
>     semi.upgrade()
> })
> 
> $("#whiteTheme").click(() => {
>    whiteTheme.applyTheme()
> })
> 
> $("#darkTheme").click(() => {
>     darkTheme.applyTheme()
> })
>
> $("#daculaTheme").click(() => {
>     daculaTheme.applyTheme()
> })
>
> $("#vueTheme").click(() => {
>     vueTheme.applyTheme()
> })
> 
> $("#vscodeTheme").click(() => {
>     vscodeTheme.applyTheme()
> })
> 
> $("#githubWhiteTheme").click(() => {
>    githubWhiteTheme.applyTheme()
> })
> 
> $("#githubDarkTheme").click(() => {
>     githubDarkTheme.applyTheme()
> })
> ```

***
