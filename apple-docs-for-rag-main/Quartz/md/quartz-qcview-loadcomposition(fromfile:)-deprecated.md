

- Quartz
- QCView
-  loadComposition(fromFile:) Deprecated

Instance Method

# loadComposition(fromFile:)

Loads the composition file located at the specified path.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func loadComposition(fromFile path: String!) -> Bool
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`path`  

A string that specifies the location of a Quartz Composer composition file.

## Return Value

If unsuccessful, returns false; any composition that’s already loaded in the view remains loaded.

## See Also

### Loading a Composition

func load(QCComposition!) -> Bool

Loads a QCComposition object into the view.

Deprecated

func loadedComposition() -> QCComposition!

Returns the composition loaded in the view.

Deprecated

func unloadComposition()

Unloads the composition from the view.

Deprecated

