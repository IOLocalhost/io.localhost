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

## Use
With the first steps we will easily create a menu with a single value

**Following the Steps**
- [ ] Create a constant with any name.
- [ ] Using the constant to build the menu.
- [ ] Creating the Button and function ID.
- [ ] Create function.

### Stage (1)
Create a constant with any name.
```js
const example = new MenuBuild()
```
- [x] Create a constant with any name. ( Done )


### Stage (2) 
Using the constant to build the menu.
```js
example.mount()
```
- [x] Create a constant with any name. ( Done )
- [x] Using the constant to build the menu. ( Done )


### Stage (3)
Creating the Button and function ID.
```js
example.addItem("Hello World","hello")
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

> Code
> ```js
> const example = new MenuBuild()
> example.mount()
> example.addItem("Hello World", "hello")
> $("#hello").click(() => { alert('Hello World')})
