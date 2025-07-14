

- WebKit JS
- CanvasRenderingContext2D
-  restore 

Instance Method

# restore

Restores the last saved set of context settings.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
void restore();
```

## Discussion

You can save and restore all of the context settings: rotation, scale, translation, transformation matrix, stroke and fill styles, and text settings. This is a very fast, nestable operation.

## See Also

### Saving and Restoring Settings

save

Saves the current context settings on the stack.

