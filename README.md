# &lt;web-loader&gt;

Web Component Loaders/Spinners in CSS3 [Web Loader] using Polymer.

## Demo
> [Check it live](http://ifly9.com.br/webcomponents/web-loader/).

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install web-loader --save
```

Or [download as ZIP](https://github.com/mvaldetaro/web-loader/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

  ```html
<script src="bower_components/platform/platform.js"></script>
  ```

2. Import Custom Element:

  ```html
<link rel="import" href="bower_components/web-loader/src/web-loader.html">
  ```

3. Start using it!

  ```html
<web-loader></web-loader>
  ```

## Options

Attribute | Options         | Default                    | Description
---       | ---             | ---                        | ---
`type`    | `circle`, `dot`, `clock` | `circle`                   | The type of loader
`display` | `block`, `none` | `block`                  | The visibility of loader
`styleOverride` | `web-loader`, `anything-else` | `web-loader`  | Specifies the reference ID of the core-style to use for overriding default stylings

## Styling

Styling is done through the use of a core-style element. All you have to do is declare a core-style element in your site with an ID that matches the `styleOverride` property of the `web-loader` component (defaults to `web-loader`). 
For example:
```html
  <core-style id="web-loader">
      .circle{
        border: 3px solid #333333;
      }
      .circle:after{
        background-color: #333333;
      }
      .clock{
        border: 3px solid #333333;
      }
      .clock:after{
        background-color: #333333;
      }
      .clock:before{
        background-color: #333333;
      }
      .dot{
        background-color: #333333;
      }
      .dot:before{
        background-color: #333333;
      }
      .dot:after{
        background-color: #333333;
      }
  </core-style>
  ```

## Browser Support

![IE](https://raw.github.com/paulirish/browser-logos/master/internet-explorer/internet-explorer_48x48.png) | ![Chrome](https://raw.github.com/paulirish/browser-logos/master/chrome/chrome_48x48.png) | ![Firefox](https://raw.github.com/paulirish/browser-logos/master/firefox/firefox_48x48.png) | ![Opera](https://raw.github.com/paulirish/browser-logos/master/opera/opera_48x48.png) | ![Safari](https://raw.github.com/paulirish/browser-logos/master/safari/safari_48x48.png)
--- | --- | --- | --- | --- |
IE 10+ ✔ | Latest ✔ | Latest ✔ | Latest ✔ | Latest ✔ |

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

Check [Release](https://github.com/mvaldetaro/web-loader/releases) list.

## License

[MIT License](http://mvaldetaro.mit-license.org/) © Magno Valdetaro
