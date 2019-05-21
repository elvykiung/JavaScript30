# Flex Panel Gallery

## Table of contents

- [General info](#general-info)
- [Code Overview](#Code-Overview)
- [JavaScript Function explain](#JavaScript-Function-explain)
- [HTML layout](#HTML-layout)
- [CSS style](#CSS-style)

## General info

![Image]()

## Code Overview

### Summary

- display: flex
- flex-direction
- justify-content
- align-items
- transform: translateX/translateY
- element.classList.toggle()
- transitionend

## CSS style

- display : flex >>to display side by side
- flex: 1 >>> equaly sizing the width
- flex: 1 0 auto >>> equal sizing height
- flex: 5 >> sizing 5 times more space than reqular
- .panel `> *` >>> access each element in side the div

- flex-direction: column >> dispaly vetically

- transform: translateY(100%) >> move away from original location

## JavaScript Function explain

```
 //  function that add class open

      function toggleOpen() {
        this.classList.toggle('open');
      }
```

```
// listening to click event and add toggleOpen function if event happend

    panels.forEach(panel => panel.addEventListener('click', toggleOpen));

```

## HTML layout
