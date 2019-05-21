# Flex Panel Gallery

## Table of contents

- [General info](#general-info)
- [Code Overview](#Code-Overview)
- [HTML layout](#HTML-layout)
- [CSS style](#CSS-style)
- [JavaScript Function explain](#JavaScript-Function-explain)

## General info

![Image](img/final.gif)

## Code Overview

### Summary

- display: flex
- flex-direction
- justify-content
- align-items
- transform: translateX/translateY
- element.classList.toggle()
- transitionend

## HTML layout

We are giving html page with DOM like below. Currently the images are display horizontally and we want to display it vertically with animation of resizing when user click on the page

```
<div class="panels">
  <div class="panel panel1">
    <p>Hey</p>
    <p>Let's</p>
    <p>Dance</p>
  </div>
  <div class="panel panel2">
  </div>
  <div class="panel panel3">
  </div>
  <div class="panel panel4">
  </div>
  <div class="panel panel5">
  </div>
</div>
```

## CSS style

- display : flex >>to display side by side
- flex: 1 >>> equally sizing the width
- flex: 1 0 auto >>> equal sizing height
- flex: 5 >>> sizing 5 times more space than regular
- .panel `> *` >>> access each element in side the div

- flex-direction: column >>> display vertically

- transform: translateY(100%) >>> move away from original location

## JavaScript Function explain

```
 //  function that add class open

      function toggleOpen() {
        this.classList.toggle('open');
      }
```

```
// listening to click event and add toggleOpen function if event happened

    panels.forEach(panel => panel.addEventListener('click', toggleOpen));

```
