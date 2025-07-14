

- Quartz
- QCView
-  load(\_:) Deprecated

Instance Method

# load(\_:)

Loads a QCComposition object into the view.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func load(_ composition: QCComposition!) -> Bool
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`composition`  

The QCComposition object to load.

## Return Value

true if successful; otherwise false. If unsuccessful, any composition that’s already loaded in the view remains loaded.

## See Also

### Loading a Composition

func loadComposition(fromFile: String!) -> Bool

Loads the composition file located at the specified path.

Deprecated

func loadedComposition() -> QCComposition!

Returns the composition loaded in the view.

Deprecated

func unloadComposition()

Unloads the composition from the view.

Deprecated

