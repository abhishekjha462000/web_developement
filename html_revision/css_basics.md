# CSS

CSS stands for cascading style sheet. It is not a programming language nor it is a markdown language like HTML.
It is used to style the documents like HTML.

There are 3 ways by which we can include CSS in our html file.

1. Inline CSS
    - This is done by using the `style` attribute inside an element. This is very specific and we only use this for testing purpose.
2. Internal CSS
    - This is the CSS which is written inside the `style` tag which is included in the `head` tag of HTML.
3. External CSS
    - This is the most feasible way. We make a seperate file in which we write all our CSS code. This file is saved using the `.css` extension.
    - This is included in the HTML file using the `link` tag.
        ```HTML
            <link rel="stylesheet" href="style.css">
        ```

## Power battle

The inline CSS has the highest priority amongst all the 3 types that we discussed. Within the internal and external CSS, it is dependent
on the order. Whichever comes latter wins.

```HTML
    <style>
        h1{
            background-color:green;
        }
    </style>
    <link rel="stylesheet" href="style.css"> 
```
In the above code snippet, the `link` tag overwrites the CSS of the style tag.

## Anatomy of CSS 

A CSS file consists of many rulesets. A CSS ruleset is a combination of selector and a declaration block. Within a declaration block,
we mention multiple declarations(also called as CSS rule), each of which is seperated via semicolon. A declaration is property-value pair.

The declrations are enclosed within a pair of open and closed curly braces. `{}`

```CSS
    p {
        background-color : green;
        color: black;
    }
```

In the above code snippet, `p` is the selector. Within the declaration block we have 2 CSS rules(declarations). The first rule has the property name `background-color` and value as `green`. The second rule has the property name `color` and value as `black`.