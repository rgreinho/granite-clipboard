# granite-clipboard

A lightweight element wrapping-up [clipboard.js](https://clipboardjs.com/)

This branch contains the Polymer 2.x class-based version of the element.


## Doc & demo

[https://lostinbrittany.github.io/granite-clipboard](https://lostinbrittany.github.io/granite-clipboard)


## Usage example

<!--
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="granite-clipboard.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<granite-clipboard text="Copy me!" verbose>
  <paper-icon-button icon="content-copy" title="copy"></paper-icon-button>
</granite-clipboard>
```



## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install LostInBrittany/granite-clipboard#polymer-2.x --save
```

Or [download as ZIP](https://github.com/LostInBrittany/granite-clipboard/archive/gh-pages.zip).

## Usage

1. Import Web Components' polyfill (if needed):

    ```html
    <script src="../bower_components/webcomponentsjs/webcomponents.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="../bower_components/granite-clipboard/granite-clipboard.html">
    ```

3. Start using it!

## Attributes

Attribute     | Type      | Default  | Description
---           | ---       | ---      | ---
`text`        | *String*  | ``       | The text to copy
`action`      | *String*  | `copy`   | The action to do (either `copy` or `cut`)


## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

### Testing the element

The element can be tested locally using the `polymer test` command.

If you do not want to setup the test tools locally, you can use the [loannister/web-devtools](https://hub.docker.com/r/loannister/web-devtools/) Docker container (currently only supports firefox 52, but more browsers are coming).

Simply run:
```
docker run -t -v=$(pwd):/code --rm --privileged loannister/web-devtools:1.2.0 polymer test
```

## License

[MIT License](http://opensource.org/licenses/MIT)
