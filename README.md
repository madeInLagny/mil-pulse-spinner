# \<mil-pulse-spinner\>

'mil-pulse-spinner' is a loading spinner that exposes a pulse animation. It uses lit-element and can be used with any webcomponent.

Demo: https://stackblitz.com/edit/mil-pulse-spinner-example?file=index.js

## Usage

### Install from npm

```sh
npm install --save mil-pulse-spinner
```

### Import to your webcomponent

```js
import "mil-pulse-spinner";
```

### Add to html

```js
<mil-pulse-spinner id="myMilPulseSpinner"></mil-pulse-spinner>
```

### Remove element when needed

When loading is complete, simply remove the element.

```js
const spinner = this.shadowRoot.getElementById("myMilPulseSpinner");

targetElement.addEventListener("loaded", function() {
  spinner.remove();
});
```

## Styling

Use customs CSS properties for styling.

| CSS property | Default | 
| -------------------- | ------- |
| `--color1` | Black | 
| `--color2` | White |
| `--width` | 40px  |
| `--height`   | 40px  |
