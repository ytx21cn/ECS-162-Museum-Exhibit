# ECS 162 Assignment 2: Museum Exhibition Responsive Page
	
## How we designed the CSS classes

### Sources consulted

We have noted the difficulties of writing and maintaining CSS rules when the CSS files grow larger and larger.

To separate responsibilities of classes and to prevent scope leaking, we have consulted some coding styles described on these pages:

- [Writing modular CSS (Part 1) — BEM](https://zellwk.com/blog/css-architecture-1)
- [Writing modular CSS (Part 2) — Namespaces](https://zellwk.com/blog/css-architecture-2/)
- [BEM naming](http://getbem.com/naming/)
- [CSS Naming Conventions that Will Save You Hours of Debugging](https://medium.freecodecamp.org/css-naming-conventions-that-will-save-you-hours-of-debugging-35cea737d849)

### Prefixing

We used prefixing to separate the responsibilities of each class and group relevant rules together. Here are the prefixes we have used:

- `.l-` for **layout**: layout rules such as margins, paddings, object alignments and flexbox rules.
- `.c-` for **component**: context-aware rules for internal states of a block, such as font sizes, colors, etc. May contain other components or objects.
- `.o-` for **object**: the minimal reusable parts that may not contain any other components or objects.
- `.data-js-`: indicate that this class is a descendant of an element that has a `data-*` attribute manipulated by JavaScript, and is dependent on the state of that `data-*` attribute.
- `t-` for **theme**: separate thematic rules such as font families, colors, all-lowercase rendering, etc.
- `u-` for **utility**: utility classes, such as designating that an element is only visible / invisible on specific devices (mobile phone / tablet / PC).
