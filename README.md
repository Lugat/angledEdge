# angledEdge
angledEdge simplified

creates angeled edges with transparent background and allows to set opacity, width and height

you must speficy the element which will contain the angled edge:

```
div {
  @include angledEdge('upper left', $color, 10%, 100%);
  
  &:before {
    @include angledEdge('upper left', $color, 10%, 100%);
  }
  
  &:after {
    @include angledEdge('lower left', $color, 100%, 100%);
  }
  
}
```

the hypotenuse can be one of the following:

* upper left
* upper right
* lower left
* lower right
