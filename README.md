[![Published on webcomponents.org][webcomponents-image]][webcomponents-url]

# \<s-table\>

Responsive HTML table extended with Polymer and Material Design.

- `<s-table>` is an HTML `<table>` element that has responsive width and optional attribute for fixed first column.
- `<s-table-lite>` is an HTML `<table>` element that don't implement Material Design.
- `<s-tbody>` and `<s-tr>` are HTML elements extended with `<iron-selector>`.

## Demo

[Full demo][webcomponents-demo]

## Usage

<!--
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="s-table-lite.html">
    <link rel="import" href="s-tbody.html">
    <link rel="import" href="s-tr.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<style>
  td, th {
    padding: 8px;
    box-sizing: border-box;
    white-space: nowrap;
  }
  td:nth-of-type(1),
  th:nth-of-type(1) {
    background-color: rgba(255, 0, 255, 0.2);
  }
  tr.iron-selected td {
    background-color: rgba(0, 0, 0, 0.1);
  }
  tr:hover td {
    background-color: rgba(0, 0, 0, 0.2);
  }
  tr td.iron-selected:not(:nth-of-type(1)) {
    background-color: rgba(255, 255, 0, 0.2);
  }
</style>

<table is="s-table-lite" fixed-column>
  <thead>
    <tr>
      <th>First Name</th>
      <th>Last Name</th>
      <th>Job Title</th>
      <th>Favorite Color</th>
      <th>Wars or Trek?</th>
      <th>Porn Name</th>
      <th>Date of Birth</th>
      <th>Dream Vacation City</th>
      <th>GPA</th>
      <th>Arbitrary Data</th>
    </tr>
  </thead>
  <tbody is="s-tbody">
    <tr is="s-tr" multi>
      <td>James</td>
      <td>Matman</td>
      <td>Chief Sandwich Eater</td>
      <td>Lettuce Green</td>
      <td>Trek</td>
      <td>Digby Green</td>
      <td>January 13, 1979</td>
      <td>Gotham City</td>
      <td>3.1</td>
      <td>RBX-12</td>
    </tr>
    <tr is="s-tr" multi>
      <td>The</td>
      <td>Tick</td>
      <td>Crimefighter Sorta</td>
      <td>Blue</td>
      <td>Wars</td>
      <td>John Smith</td>
      <td>July 19, 1968</td>
      <td>Athens</td>
      <td>N/A</td>
      <td>Edlund, Ben (July 1996).</td>
    </tr>
    <tr is="s-tr" multi>
      <td>Jokey</td>
      <td>Smurf</td>
      <td>Giving Exploding Presents</td>
      <td>Smurflow</td>
      <td>Smurf</td>
      <td>Smurflane Smurfmutt</td>
      <td>Smurfuary Smurfteenth, 1945</td>
      <td>New Smurf City</td>
      <td>4.Smurf</td>
      <td>One</td>
    </tr>
    <tr is="s-tr" multi>
      <td>Cindy</td>
      <td>Beyler</td>
      <td>Sales Representative</td>
      <td>Red</td>
      <td>Wars</td>
      <td>Lori Quivey</td>
      <td>July 5, 1956</td>
      <td>Paris</td>
      <td>3.4</td>
      <td>3451</td>
    </tr>
    <tr is="s-tr" multi>
      <td>Captain</td>
      <td>Cool</td>
      <td>Tree Crusher</td>
      <td>Blue</td>
      <td>Wars</td>
      <td>Steve 42nd</td>
      <td>December 13, 1982</td>
      <td>Las Vegas</td>
      <td>1.9</td>
      <td>Under the couch</td>
    </tr>
  </tbody>
</table>
```

## Installation

`bower i s-table -S`

## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
$ polymer serve build/bundled
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.

## License

MIT: [StartPolymer/license](https://github.com/StartPolymer/license)

[webcomponents-image]: https://img.shields.io/badge/webcomponents.org-published-blue.svg
[webcomponents-url]: https://webcomponents.org/element/StartPolymer/s-table
[webcomponents-demo]: https://webcomponents.org/element/StartPolymer/s-table/demo/demo/s-table.html
