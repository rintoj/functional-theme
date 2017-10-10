# Functional Theme

This module will let you seamlessly create and integrate modular themes using predefined mixins. `SaSS` and `Less` configurations are available.

## Install

```bash
npm install functional-theme -S
```

## Get Started

1. Create `style.less` or `style.scss` and add each color to the theme using `addColor(name, color, contrastColor);` mixin

### If you are using less

```less
@import '../node_modules/functional-theme/index.less';

.theme1 {
  .addColor(primary, #2C3336, #d7e3ea);
  .addColor(secondary, #fafafa, #4b585f);
  .addColor(accent, #ffae27, #424242);
  .addColor(card, #fff, #000);
  .addColor(page, #fefefe, #525252);
  .addColor(divider, #263138);
  .addColor(error, #D02A2B, #fff);
  .addColor(success, #29D185, #fff);
  .addColor(warning, #ffae27, #424242);
}
```

```scss
@import '~functional-theme/index.scss';

.theme1 {
  @include addColor(primary, #2C3336, #d7e3ea);
  @include addColor(secondary, #fafafa, #4b585f);
  @include addColor(accent, #ffae27, #424242);
  @include addColor(card, #fff, #000);
  @include addColor(page, #fefefe, #525252);
  @include addColor(divider, #263138);
  @include addColor(error, #D02A2B, #fff);
  @include addColor(success, #29D185, #fff);
  @include addColor(warning, #ffae27, #424242);
}
```

2. Add name of the theme to `<body>`

```html
<body class="theme1">
  ....
</body>
```

3. Use the colors classes.

| Style | Css
|-------|---------------------------------
| .${color} | background-color: ${value}; color: ${contrast}; |
| .${color}-contrast | color: ${contrast}; |
| .${color}-text | color: ${value}; |
| .${color}-bg | background-color: ${value}; |
| .${color}-ba | border-color: ${value}; |
| .${color}-bt | border-top-color: ${value}; |
| .${color}-br | border-right-color: ${value}; |
| .${color}-bb | border-bottom-color: ${value}; |
| .${color}-bl | border-left-color: ${value}; |
| .${color}-o  | outline-left-color: ${value}; |
| .${color}-f  | fill: ${value}; |
| .${color}-s  | stroke: ${value}; |
| .${color}--hover | background-color: ${value}; color: ${contrast}; |
| .${color}-contrast--hover | color: ${contrast}; |
| .${color}-text--hover | color: ${value}; |
| .${color}-bg--hover | background-color: ${value}; |
| .${color}-ba--hover | border-color: ${value}; |
| .${color}-bt--hover | border-top-color: ${value}; |
| .${color}-br--hover | border-right-color: ${value}; |
| .${color}-bb--hover | border-bottom-color: ${value}; |
| .${color}-bl--hover | border-left-color: ${value}; |
| .${color}-o--hover  | outline-color: ${value}; |
| .${color}-f--hover  | fill: ${value}; |
| .${color}-s--hover  | stroke: ${value}; |
| .${color}--focus | background-color: ${value}; color: ${contrast}; |
| .${color}-contrast--focus | color: ${contrast}; |
| .${color}-text--focus | color: ${value}; |
| .${color}-bg--focus | background-color: ${value}; |
| .${color}-ba--focus | border-color: ${value}; |
| .${color}-bt--focus | border-top-color: ${value}; |
| .${color}-br--focus | border-right-color: ${value}; |
| .${color}-bb--focus | border-bottom-color: ${value}; |
| .${color}-bl--focus | border-left-color: ${value}; |
| .${color}-o--focus  | outline-color: ${value}; |
| .${color}-f--focus  | fill: ${value}; |
| .${color}-s--focus  | stroke: ${value}; |

## Contributing
Contributions are very welcome! Just send a pull request. Feel free to contact me or checkout my [GitHub](https://github.com/rintoj) page.

## Author

**Rinto Jose** (rintoj)

### Hope this module is helpful to you. Checkout my other [projects](https://github.com/rintoj) and [articles](https://medium.com/@rintoj). Enjoy coding!

Follow me:
  [GitHub](https://github.com/rintoj)
| [Facebook](https://www.facebook.com/rinto.jose)
| [Twitter](https://twitter.com/rintoj)
| [Google+](https://plus.google.com/+RintoJoseMankudy)
| [Youtube](https://youtube.com/+RintoJoseMankudy)

## Versions
[Check CHANGELOG](https://github.com/rintoj/functional-theme/blob/master/CHANGELOG.md)

## License
```
The MIT License (MIT)

Copyright (c) 2017 Rinto Jose (rintoj)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
