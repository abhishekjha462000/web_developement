# styling list

The `list-style-type` CSS property sets the marker (such as a disc, character, or custom counter style) of a list item element.

We can remove the default styling completely by setting the `list-style-type` to `none`.

```CSS
    ul {
        list-style-type : none;
    }
```

The following values are available:

```CSS
    /* Partial list of types */
    list-style-type: disc;
    list-style-type: circle;
    list-style-type: square;
    list-style-type: decimal;
    list-style-type: georgian;
    list-style-type: trad-chinese-informal;
    list-style-type: kannada;

    /* <string> value */
    list-style-type: "-";

    /* Identifier matching an @counter-style rule */
    list-style-type: custom-counter-style;

    /* Keyword value */
    list-style-type: none;
```