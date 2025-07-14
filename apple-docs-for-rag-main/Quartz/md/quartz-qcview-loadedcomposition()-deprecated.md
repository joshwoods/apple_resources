

- Quartz
- QCView
-  loadedComposition() Deprecated

Instance Method

# loadedComposition()

Returns the composition loaded in the view.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func loadedComposition() -> QCComposition!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The composition loaded in the view; otherwise `nil`.

## See Also

### Loading a Composition

func loadComposition(fromFile: String!) -> Bool

Loads the composition file located at the specified path.

Deprecated

func load(QCComposition!) -> Bool

Loads a QCComposition object into the view.

Deprecated

func unloadComposition()

Unloads the composition from the view.

Deprecated

