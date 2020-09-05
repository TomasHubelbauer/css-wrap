# CSS Wrapp

Making it so that the two children of a container will sit one after another as
long as they both fit length-wise. If they do not, they will sit atop one
another. If either still doesn't fit even individually, it will break lines.

## Example

Elements fit one after another:

```
 ________________________________________________________________
|                                                                |
| [first element is this element] [second element is me]         |
|________________________________________________________________|

```

Elements do not fit one after another so they sit one atop the other:

```
 _________________________________________
|                                         |
| [first element is this element]         |
| [second element is me]                  |
|_________________________________________|
```

Elements sit atop one another and also break lines as needed independently:

```
 ______________________
 |                     |
 | [first element is]  |
 | [this element]      |
 | [second element is] |
 | [me]                |
 |_____________________|
```

## To-Do

### Fix the short-first-bug

If the first element is short and only the second element breaks lines, it will stack
next to the first element instead of flowing on the second line where the first element
didn't break line into.

I'm not sure if this is even solvable using CSS.
