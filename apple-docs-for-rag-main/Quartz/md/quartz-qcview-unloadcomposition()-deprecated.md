

- Quartz
- QCView
-  unloadComposition() Deprecated

Instance Method

# unloadComposition()

Unloads the composition from the view.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func unloadComposition()
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Discussion

If necessary, this method calls stopRendering() prior to unloading the composition.

## See Also

### Loading a Composition

func loadComposition(fromFile: String!) -> Bool

Loads the composition file located at the specified path.

Deprecated

func load(QCComposition!) -> Bool

Loads a QCComposition object into the view.

Deprecated

func loadedComposition() -> QCComposition!

Returns the composition loaded in the view.

Deprecated

