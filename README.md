# \<etools-content-toggle-button\>

Toggle button with icon used to show or hide different content, for example an iron-collapse element.

## Usage
```html
<etools-content-toggle-button label="Toggle content" active="{{opened}}"></etools-content-toggle-button>
<iron-collapse opened="[[opened]]">
Some collapsible content...
</iron-collapse>

<etools-content-toggle-button label="Toggle content" active="{{opened}}" is-disabled="true"></etools-content-toggle-button>
```

Available attributes:
* label: String, the element label
* active: Boolean, content status, if true, content is shown
* isDisabled: Boolean, disabled state

## Styling

You can use defined variables to change button style.

Custom property | Description | Default
----------------|-------------|----------
`--etools-content-toggle-btn-color` | Element text color | `#4a90e2`
`--etools-content-toggle-btn-icon-color` | Icon color | `#9b9b9b`
`--etools-content-toggle-btn-font-size` | Element text font size | `14px`
`--etools-content-toggle-btn-disabled-color` | Disabled element color | `#9b9b9b`
`--etools-content-toggle-btn` | Mixin applied to button | `{}`
## Install
```bash
$ bower install --save etools-content-toggle-button
```

## Preview element locally
Install needed dependencies by running: `$ bower install`.
Make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `$ polymer serve` to serve your element application locally.

## Linting the code

Innstall local npm packages (run `npm install`)
Then just run the linting task

```bash
$ npm run lint
```
You should also use polylint. If you don't have Polylint installed run `npm install -g polylint`.
Then just run the linter on each file you wish to check like so

```bash
$ polylint -i filename.html
```
At the moment polylint crashes if it encounters a missing import. If that happens, temporarily comment out such imports and run the command again.

## Running Tests

```
$ polymer test
```
