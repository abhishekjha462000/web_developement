# relative position

1. Element fits in the normal flow of the document.
2. top, right, bottom, left and z-index can be used to scoot the element from its default spot.
3. Even if the element is offset, its original space in the document is still maintained.

## Example

Consider the following HTML code
```HTML
<p>
  Lorem, ipsum dolor sit amet consectetur adipisicing elit. Suscipit saepe
  facere reprehenderit porro, sed provident ex labore? Explicabo, quia dolore.
  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae, eveniet.
</p>

<p id="special">
  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Commodi, explicabo
  sunt rem veniam exercitationem natus aspernatur dolor impedit error fuga vero,
  dolorum voluptas harum doloribus debitis sapiente neque earum voluptatibus.
</p>

<p>
  Lorem ipsum dolor sit, amet consectetur adipisicing elit. Id, animi. Dolorem
  velit eaque atque, ad fuga debitis provident quaerat tenetur pariatur
  exercitationem iure inventore magnam dolores sit harum iste nostrum?
</p>

```
Have a look at this CSS code as well
```CSS
  p {
    border: 2px solid red;
    background-color: aquamarine;
    margin: 30px;
    font-size: 2rem;
  }

  #special {
    background-color: rgb(7, 126, 206);
    font-size: 30px;
    position: relative;
    top: 10px;
    right: 30px;
  }
```

When we use `relative position`, then the `top`, `right`, `bottom`, `left` work in reference to the `original position` of the element. Also, the element does not leave its space in the normal document flow.

## Notes

1. A value of `top = 50px` is same as `bottom = -50px` and a value of `left = 20px` is same as `right = -20px`.
2. Due to the above fact no 1, a lot of people stick to `(top, left)` and  use negative values as well.
3. You could also use `(bottom, right)` and use negative values.
4. Just stay consistent.