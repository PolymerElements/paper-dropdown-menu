[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://beta.webcomponents.org/element/PolymerElements/paper-dropdown-menu)
[![Build status](https://travis-ci.org/PolymerElements/paper-dropdown-menu.svg?branch=master)](https://travis-ci.org/PolymerElements/paper-dropdown-menu)

# \<paper-dropdown-menu\>

Material design: [Dropdown menus](https://www.google.com/design/spec/components/buttons.html#buttons-dropdown-buttons)

`paper-dropdown-menu` is similar to a native browser select element.
`paper-dropdown-menu` works with selectable content. 

<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="paper-dropdown-menu.html">
    <link rel="import" href="../paper-item/paper-item.html">
    <link rel="import" href="../paper-listbox/paper-listbox.html">
    <link rel="import" href="../iron-demo-helpers/demo-pages-shared-styles.html">
    <style is="custom-style" include="demo-pages-shared-styles">
      paper-dropdown-menu, paper-listbox {
        width: 250px;
      }
      paper-dropdown-menu {
        height: 200px;
        margin: auto;
        display: block;
      }
    </style>
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->

## Examples

In Polymer 1 the content of the dropdown should be a `paper-listbox` with `class="dropdown-content"`

```html
<paper-dropdown-menu label="Dinosaurs">
  <paper-listbox class="dropdown-content" selected="1">
    <paper-item>allosaurus</paper-item>
    <paper-item>brontosaurus</paper-item>
    <paper-item>carcharodontosaurus</paper-item>
    <paper-item>diplodocus</paper-item>
  </paper-listbox>
</paper-dropdown-menu>
```

In Polymer 2 specify `slot="dropdown-content"` instead:

```html
<paper-dropdown-menu label="Dinosaurs">
  <paper-listbox slot="dropdown-content" selected="1">
    <paper-item>allosaurus</paper-item>
    <paper-item>brontosaurus</paper-item>
    <paper-item>carcharodontosaurus</paper-item>
    <paper-item>diplodocus</paper-item>
  </paper-listbox>
</paper-dropdown-menu>
```

