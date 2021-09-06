# Examples

## SOURCE
```js
// ==UserScript==
// @name         IO.Localhost LIB SRC
// @github       alexsandersilv
// @namespace    https://github.com/alexsandersilv/io.localhost/
// @version      1.0.0
// @description  Code Edit
// @author       Dazai
// @match        http://bloble.io/*
// @icon         https://io-localhost.vercel.app/favicon.ico
// @license      MIT License
// @grant        none
// ==/UserScript==
 
    const ioSection = $("<section />", {
        id: 'ioSection',
        class: 'ioSection'
    })
 
    const ioLib = $("<script />", {// code
        src: 'https://io-localhost.vercel.app/assets/javascript/lib/file.lib.js'
    })
 
    $("#darkener").append(ioSection)
    $("#ioSection").append(ioLib)
 
/*\
|*|
|*| :: Importing the library, please do not touch anything above ::
|*| :: Importando a biblioteca, por favor, não toque em nada acima ::
|*|
|*| :: Your script should be under this comment ::
|*| :: Seu script deve ficar em baixo desse comentário ::
|*|                DOCS: https://io-localhost.vercel.app
\*/// Practice
 
$("#enterGameButton").click(() => {
  // you code here
})

```

### IO.Localhost Basic Themes
```js
// ==UserScript==
// @name         IO.Localhost Basic Themes
// @github       alexsandersilv
// @namespace    https://github.com/alexsandersilv/io.localhost/
// @version      1.0.0
// @description  Basic theme and menu creation
// @author       Dazai
// @match        http://bloble.io/*
// @icon         https://io-localhost.vercel.app/favicon.ico
// @license      MIT License
// @grant        none
// ==/UserScript==
 
 
    const ioSection = $("<section />", {
        id: 'ioSection',
        class: 'ioSection'
    })
 
    const ioLib = $("<script />", {// code
        src: 'https://io-localhost.vercel.app/assets/javascript/lib/file.lib.js'
    })
 
    $("#darkener").append(ioSection)
    $("#ioSection").append(ioLib)
 
/*\
|*|
|*| :: Importing the library, please do not touch anything above ::
|*| :: Importando a biblioteca, por favor, não toque em nada acima ::
|*|
|*| :: Your script should be under this comment ::
|*| :: Seu script deve ficar em baixo desse comentário ::
|*|                DOCS: https://io-localhost.vercel.app
\*/// Practice
 
$("#enterGameButton").click(() => {
    //=====> Themes
    const whiteTheme = new Theme("#ebebeb", "#d6d6d6", "rgba(0,0,0,0.08)", "rgba(255, 0, 0, 0.1)")
    const darkTheme = new Theme( "rgb(10, 10, 10)" , "rgb(20, 20, 20)" , "#222" , "rgba(200, 0, 0, 0.5)")
    const daculaTheme = new Theme("#1e1a30", "#454545", "#bc04bf", "#04bf23")
    const vueTheme = new Theme("#35495E", "#37587a", "rgba(196, 196, 196, 0.5)", "#41B883")
    const vscodeTheme = new Theme("#242220", "#383533", "#17692b", "#009dff")
    const githubWhiteTheme = new Theme("#ebebeb", "#8a8a88", "#8f000e", "#00158f")
    const githubDarkTheme = new Theme("#0d1117", "#263142", "#7d0b7b", "#0b3b7d")
 
const menu = new MenuBuild()
menu.mount()
 
    menu.addItem("White", "whiteTheme")
    menu.addItem("Dark", "darkTheme")
    menu.addItem("Dracula", "daculaTheme")
    menu.addItem("Vue", "vueTheme")
    menu.addItem("Visual Studio Code", "vscodeTheme")
    menu.addItem("Github White", "githubWhiteTheme")
    menu.addItem("Github Dark", "githubDarkTheme")
 
    $("#whiteTheme").click(() => { whiteTheme.applyTheme() })
    $("#darkTheme").click(() => { darkTheme.applyTheme() })
    $("#daculaTheme").click(() => { daculaTheme.applyTheme() })
    $("#vueTheme").click(() => { vueTheme.applyTheme() })
    $("#vscodeTheme").click(() => { vscodeTheme.applyTheme() })
    $("#githubWhiteTheme").click(() => { githubWhiteTheme.applyTheme() })
    $("#githubDarkTheme").click(() => { githubDarkTheme.applyTheme() })
 
})
```


### IO.Localhost Basic Menu
```js
// ==UserScript==
// @name         IO.Localhost Basic Menu 
// @github       alexsandersilv
// @namespace    https://github.com/alexsandersilv/io.localhost/
// @version      1.0.2
// @description  Basic menu creation && Upgrade Item
// @author       Dazai
// @match        http://bloble.io/*
// @icon         https://io-localhost.vercel.app/favicon.ico
// @license      MIT License
// @grant        none
// ==/UserScript==
 
    const ioSection = $("<section />", {
        id: 'ioSection',
        class: 'ioSection'
    })
 
    const ioLib = $("<script />", {// code
        src: 'https://io-localhost.vercel.app/assets/javascript/lib/file.lib.js'
    })
 
    $("#darkener").append(ioSection)
    $("#ioSection").append(ioLib)
 
/*\
|*|
|*| :: Importing the library, please do not touch anything above ::
|*| :: Importando a biblioteca, por favor, não toque em nada acima ::
|*|
|*| :: Your script should be under this comment ::
|*| :: Seu script deve ficar em baixo desse comentário ::
|*|                DOCS: https://io-localhost.vercel.app
\*/// Practice
 
$("#enterGameButton").click(() => {
 
const menu = new MenuBuild()
menu.mount()
 
    menu.addItem("Upgrade Boulder", "boulder")
menu.addItem("Upgrade Spike", "spikes")
menu.addItem("Upgrade Micro-generators", "micro")
menu.nextLine()
menu.addItem("Upgrade Rapid ", "rapidTurret")
menu.addItem("Upgrade Gatling ", "gatlinTurret")
menu.addItem("Upgrade Ranged ", "rangedTurret")
menu.addItem("Upgrade Spotter", "spotterTorret")
menu.nextLine()
menu.addItem("Upgrade Anti-tank", "anti")
menu.addItem("Upgrade Semi Auto", "semi")
 
    //set item for upgrade
    const boulders = new Item("boulder")
    const spikes = new Item("spikes")
    const micro = new Item("micro")
    const rapid = new Item("rapid")
    const gatl = new Item("gatlin")
    const ranged = new Item("ranged")
    const spo = new Item("spotter")
    const anti = new Item("anti")
    const semiauto = new Item("semi")
 
    //function
    $("#boulder").click(() => {
        boulders.upgrade()
    })
    $("#spikes").click(() => {
        spikes.upgrade()
    })
    $("#micro").click(() => {
        micro.upgrade()
    })
 
    $("#rapidTurret").click(() => {
        rapid.upgrade()
    })
    $("#gatlinTurret").click(() => {
        gatl.upgrade()
    })
    $("#rangedTurret").click(() => {
        ranged.upgrade()
    })
    $("#spotterTorret").click(() => {
        spo.upgrade()
    })
 
    $("#anti").click(() => {
        anti.upgrade()
    })
 
    $("#semi").click(() => {
        semi.upgrade()
    })
 
 
})
```

### Complete 
```js
// ==UserScript==
// @name         IO.Localhost LIB
// @github       alexsandersilv
// @namespace    https://github.com/alexsandersilv/io.localhost/
// @version      1.0.0
// @description  Bloble for Devs
// @author       Dazai
// @match        http://bloble.io/*
// @icon         https://io-localhost.vercel.app/favicon.ico
// @license      MIT License
// @grant        none
// ==/UserScript==
 
 
    const ioSection = $("<section />", {
        id: 'ioSection',
        class: 'ioSection'
    })
 
    const ioLib = $("<script />", {// code
        src: 'https://io-localhost.vercel.app/assets/javascript/lib/file.lib.js'
    })
 
    $("#darkener").append(ioSection)
    $("#ioSection").append(ioLib)
 
 
/*
//EN
Example of use: Create Theme
--> Creating a new theme quickly.
 
const darkTheme = new Theme( "rgb(10, 10, 10)" , "rgb(20, 20, 20)" , "#222" , "rgba(200, 0, 0, 0.5)")
darkTheme.applyTheme() // New theme created
 
 
HUEHUE
Exemplo de uso: Criar Tema
--> Criar um novo tema rapidamente.
 
const darkTheme = new Theme( "rgb(10, 10, 10)" , "rgb(20, 20, 20)" , "#222" , "rgba(200, 0, 0, 0.5)")
darkTheme.applyTheme() // Novo tema já criado
----------------------------------------------
 
EN
Example of use: Game Processing (Memory Usage)
--> Changing game memory usage, play on ultra.
 
const ultraProcess = new GameProcess("ultra")
ultraProcess.run()
 
Note: This is the processing list you can use.
1- Ultra - ultra
2- Maximum - max
3- Normal - normal
4- Minimum - low
 
HUEHUE
Exemplo de uso: processamento de jogo (uso de memória)
--> Alterar o uso de memória do jogo, jogar no ultra.
 
const ultraProcess = new GameProcess("ultra")
ultraProcess.run()
 
Observação: esta é a lista de processamento que você pode usar.
1- Ultra - ultra
2- Maximum - max
3- Normal - normal
4- Minimum - low
----------------------------------------------
 
EN
Example of use: Item Upgrade
--> Item update
 
const generators = new Item("gen")
const microGen = new Item("micro")
const wall = New Item("boulder")
 
generators.upgrade()
microGen.upgrade()
wall.upgrade()
keep going ...
 
HUEHUE
Exemplo de uso: Upgrade de Item
--> Atualização de item
 
const generators = new Item("gen")
const microGen = new Item("micro")
const wall = New Item("boulder")
 
generators.upgrade()
microGen.upgrade()
wall.upgrade()
 
Assim por diante...
----------------------------------------------
 
EN
Example of use: Create Menu
--> Assembling the Menu
 
const menu = new MenuBuild()
const menu.mount()
 
--> Adding Items and Their Function Values
 
menu.addItem("Power", "genUpgrade")
menu.addItem("Micro-Gen", "microUpgrade")
menu.addItem("Boulder", "boulders")
 
--> Line break
menu.nextLine()
 
--> If you want to add more items
menu.addItem("ItemName", "ItemNameFunc")
menu.addItem("ItemName", "ItemNameFunc")
menu.addItem("ItemName", "ItemNameFunc")
keep going ...
 
HUEHUE
Exemplo de uso: Criar Menu
--> Montagem do Menu
 
const menu = new MenuBuild()
const menu.mount()
 
--> Adicionar itens e seus valores de função
menu.addItem("Power", "genUpgrade")
menu.addItem("Micro-Gen", "microUpgrade")
menu.addItem("Boulder", "boulders")
 
--> Quebra de linha
menu.nextLine()
 
--> Se você quiser adicionar mais itens
menu.addItem("ItemName", "ItemNameFunc")
menu.addItem("ItemName", "ItemNameFunc")
menu.addItem("ItemName", "ItemNameFunc")
Assim por diante...
 
/*\
|*|
|*| :: Importing the library, please do not touch anything above ::
|*| :: Importando a biblioteca, por favor, não toque em nada acima ::
|*|
|*| :: Your script should be under this comment ::
|*| :: Seu script deve ficar em baixo desse comentário ::
|*|                DOCS: https://io-localhost.vercel.app
\*/// Practice
 
$("#enterGameButton").click(() => {
    //=====> Themes
    const darkTheme = new Theme( "rgb(10, 10, 10)" , "rgb(20, 20, 20)" , "#222" , "rgba(200, 0, 0, 0.5)")
    const whiteTheme = new Theme("#ebebeb", "#d6d6d6", "rgba(0,0,0,0.08)", "rgba(255, 0, 0, 0.1)")
 
    //=====> Upgrade List
    // gens
    const power = new Item("power")
 
    // walls
    const bould = new Item("boulders")
    const spikes = new Item("spikes")
    const micro = new Item("micro")
 
    //=====> Basic Menu
    const menu = new MenuBuild()
    menu.mount()
 
    // line 0
    menu.addItem("Upgrade: Boulders", "boulderUpgrade")
    menu.addItem("Upgrade: Spikes", "spikesUpgrade")
    menu.addItem("Upgrade: Micro", "microUpgrade")
 
    // next line (1)
    menu.nextLine()
 
    //line 1
    menu.addItem("Power Plants", "power")
 
    // next line (2)
    menu.nextLine()
 
    //line 2
    menu.addItem("Theme: White", "white")
    menu.addItem("Theme: Dark", "dark")
 
    // functions
    $("#boulderUpgrade").click(() => {
        bould.upgrade()
    })
 
    $("#spikesUpgrade").click(() => {
        spikes.upgrade()
    })
 
    $("#microUpgrade").click(() => {
        micro.upgrade()
    })
 
    $("#power").click(() => {
        power.upgrade()
    })
 
    $("#white").click(() => {
        whiteTheme.applyTheme()
    })
 
    $("#dark").click(() => {
        darkTheme.applyTheme()
    })
})
```
