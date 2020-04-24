# Mixins

Most mixins contain the same signature and come with sensible defaults.  You can override anyone of them; some on a global level by overriding the configuration that is passed in, but the `$className` is unique to each mixin and defaults to the name of the property being used.  For example if you're using `animation-direction()` mixin, then the default class name would be `animation-direction`.

Some mixins will have other parameters but for the most part they all contain
these following:

| Name           | Type                                                             | Description                                   | Default               |
| :------------- | :--------------------------------------------------------------- | :-------------------------------------------- | :-------------------- |
| `$className`   | **[String](https://sass-lang.com/documentation/values/strings)** | a CSS class name that will be used            | `<property name>`     |
| `$breakpoints` | **[Map](https://sass-lang.com/documentation/values/maps)**       | a map of grid breakpoints                     | `config.$breakpoints` |
