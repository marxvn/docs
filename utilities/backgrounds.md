# Backgrounds

## Background Attachment

Utilities for controlling how a background image behaves when scrolling.

| Class | Properties |
| :---- | :--------- |
| bg-fixed | background-attachment: fixed; |
| bg-local | background-attachment: local; |
| bg-scroll | background-attachment: scroll; |

## Background Clip

Utilities for controlling the bounding box of an element's background.

| Class | Properties |
| :---- | :--------- |
| bg-clip-border | background-clip: border-box; |
| bg-clip-padding | background-clip: padding-box; |
| bg-clip-content | background-clip: content-box; |
| bg-clip-text | background-clip: text; |

## Background Color

Utilities for controlling an element's background color.

| Class | Properties |
| :---- | :--------- |
| bg-transparent | background-color: transparent; |
| bg-current | background-color: currentColor; |
| `bg-${color}` | --tw-bg-opacity: 1;<br>background-color: `rgba(R, G, B, var(--tw-bg-opacity));` |

<Customizing>

```js
// windi.config.js
export default {
  theme: {
    backgroundColor: theme => ({
      ...theme('colors'),
      primary: '#3490dc',
      secondary: '#ffed4a',
      danger: '#e3342f',
    }),
  },
}
```

</Customizing>

## Background Opacity

Utilities for controlling the opacity of an element's background color.

| Class | Properties |
| :---- | :--------- |
| `bg-opacity-${int<=100}` | --tw-bg-opacity: `${int/100};` |

<Customizing>

```js
// windi.config.js
export default {
  theme: {
    extend: {
      opacity: {
        light: '0.15',
      },
    },
  },
}
```

</Customizing>

## Background Position

Utilities for controlling the position of an element's background image.

| Class | Properties |
| :---- | :--------- |
| bg-bottom | background-position: bottom; |
| bg-center | background-position: center; |
| bg-left | background-position: left; |
| bg-left-bottom | background-position: left bottom; |
| bg-left-top | background-position: left top; |
| bg-right | background-position: right; |
| bg-right-bottom | background-position: right bottom; |
| bg-right-top | background-position: right top; |
| bg-top | background-position: top; |

<Customizing>

```js
// windi.config.js
export default {
  theme: {
    backgroundPosition: {
      'bottom': 'bottom',
      'bottom-4': 'center bottom 1rem',
      'center': 'center',
      'left': 'left',
      'left-bottom': 'left bottom',
      'left-top': 'left top',
      'right': 'right',
      'right-bottom': 'right bottom',
      'right-top': 'right top',
      'top': 'top',
      'top-4': 'center top 1rem',
    },
  },
}
```

</Customizing>

## Background Repeat

Utilities for controlling the repetition of an element's background image.

| Class | Properties |
| :---- | :--------- |
| bg-repeat | background-repeat: repeat; |
| bg-no-repeat | background-repeat: no-repeat; |
| bg-repeat-x | background-repeat: repeat-x; |
| bg-repeat-y | background-repeat: repeat-y; |
| bg-repeat-round | background-repeat: round; |
| bg-repeat-space | background-repeat: space; |

## Background Size

Utilities for controlling the background size of an element's background image.

| Class | Properties |
| :---- | :--------- |
| bg-auto | background-size: auto; |
| bg-cover | background-size: cover; |
| bg-contain | background-size: contain; |

<Customizing>

```js
export default {
  theme: {
    backgroundSize: {
      'auto': 'auto',
      'cover': 'cover',
      'contain': 'contain',
      '50%': '50%',
      '16': '4rem',
    },
  },
}
```

</Customizing>

## Background Image

Utilities for controlling an element's background image.

| Class | Properties |
| :---- | :--------- |
| bg-none | background-image: none; |
| bg-gradient-to-t | background-image: linear-gradient(to top, var(--tw-gradient-stops)); |
| bg-gradient-to-tr | background-image: linear-gradient(to top right, var(--tw-gradient-stops)); |
| bg-gradient-to-r | background-image: linear-gradient(to right, var(--tw-gradient-stops)); |
| bg-gradient-to-br | background-image: linear-gradient(to bottom right, var(--tw-gradient-stops)); |
| bg-gradient-to-b | background-image: linear-gradient(to bottom, var(--tw-gradient-stops)); |
| bg-gradient-to-bl | background-image: linear-gradient(to bottom left, var(--tw-gradient-stops)); |
| bg-gradient-to-l | background-image: linear-gradient(to left, var(--tw-gradient-stops)); |
| bg-gradient-to-tl | background-image: linear-gradient(to top left, var(--tw-gradient-stops)); |

<Customizing>

```js
// windi.config.js
export default {
  theme: {
    extend: {
      backgroundImage: theme => ({
        'hero-pattern': 'url(\'/img/hero-pattern.svg\')',
        'footer-texture': 'url(\'/img/footer-texture.png\')',
      }),
    },
  },
}
```

</Customizing>

## Gradient Color Stops

Utilities for controlling the color stops in background gradients.

| Class | Properties |
| :---- | :--------- |
| from-transparent | --tw-gradient-from: transparent;<br>--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to, rgba(0, 0, 0, 0)); |
| from-current | --tw-gradient-from: currentColor;<br>--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to, rgba(255, 255, 255, 0)); |
| `from-${color}` | --tw-gradient-from: `${hex};`<br>--tw-gradient-stops: `var(--tw-gradient-from), var(--tw-gradient-to, rgba(R, G, B, 0));` |

## Background Blend Mode

Utilities for controlling how an element's background image should blend with its background color.

| Class                | Properties                          |
| :------------------- | :---------------------------------- |
| bg-blend-normal      | background-blend-mode: normal;      |
| bg-blend-multiply    | background-blend-mode: multiply;    |
| bg-blend-screen      | background-blend-mode: screen;      |
| bg-blend-overlay     | background-blend-mode: overlay;     |
| bg-blend-darken      | background-blend-mode: darken;      |
| bg-blend-lighten     | background-blend-mode: lighten;     |
| bg-blend-color-dodge | background-blend-mode: color-dodge; |
| bg-blend-color-burn  | background-blend-mode: color-burn;  |
| bg-blend-hard-light  | background-blend-mode: hard-light;  |
| bg-blend-soft-light  | background-blend-mode: soft-light;  |
| bg-blend-difference  | background-blend-mode: difference;  |
| bg-blend-exclusion   | background-blend-mode: exclusion;   |
| bg-blend-hue         | background-blend-mode: hue;         |
| bg-blend-saturation  | background-blend-mode: saturation;  |
| bg-blend-color       | background-blend-mode: color;       |
| bg-blend-luminosity  | background-blend-mode: luminosity;  |
