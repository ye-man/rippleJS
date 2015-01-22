# rippleJS

Adds Material Design-style feedback ripples to your existing HTML without any dependencies. [Show me the demos!](http://samthor.github.io/rippleJS)

## Usage

Include the [rippleJS script](https://cdn.rawgit.com/samthor/rippleJS/v1.0.0/ripple.min.js) at the end of your page. Then, add element with the `rippleJS` class within a parent element that has layout (aka, `position: relative` or `position: absolute`).

```html
<button class="yourButton">
  Click Me
  <link class="rippleJS" />
</button>

<script src="https://cdn.rawgit.com/samthor/rippleJS/master/ripple.min.js"></script>
```

rippleJS adds handlers on `document.body`, so you don't need to register any new elements as you add them to the DOM. It supports touch and mouse events, and includes its own CSS.

### Ripple Fill

By adding the `fill` class to a `rippleJS` element, the rippler will fill to rounded corners, good for form elements with fixed size. For example:

```html
<div class="optHolder">
  <input type="checkbox" />
  <link class="rippleJS fill" />
</div>
```

### Ripple Color

To change the default color of a ripple, add the following style rule:

```css
.rippleJS .ripple {
  background: red;
}
```

You could also change it just for some elements:

```css
.yourClassName .rippleJS .ripple {
  background: blue;
}
```

## Supports

Chrome, Safari, Firefox (all as of Dec 2014).

## Bower

Instead of using rippleJS directly, you can fetch it using Bower:

    $ bower install vanilla-ripplejs
