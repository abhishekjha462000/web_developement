# id selector

The CSS ID selector matches an element based on the value of the element's id attribute. In order for the element to be selected, its id attribute must match exactly the value given in the selector.

```CSS
    #identified {
        background-color: skyblue;
    }
```

Syntactically (but not specificity-wise), this is equivalent to the following attribute selector:

```CSS
    [id="identified"]{
        background-color: skyblue;
    }
```

# class selector

The CSS class selector matches elements based on the contents of their class attribute.

```CSS
    /* All elements with class="spacious" */
    .spacious { /* This is similar to [class~="spacious"]*/
    margin: 2em;
    }

    /* All <li> elements with class="spacious" */
    li.spacious {
    margin: 2em;
    }

    /* All <li> elements with a class list that includes both "spacious" and "elegant" */
    /* For example, class="elegant retro spacious" */
    li.spacious.elegant {
    margin: 2em;
    }
```

