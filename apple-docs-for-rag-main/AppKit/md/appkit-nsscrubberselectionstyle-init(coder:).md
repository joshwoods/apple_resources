

- AppKit
- NSScrubberSelectionStyle
-  init(coder:) 

Initializer

# init(coder:)

Initializes a scrubber selection style when included from a nib or Storyboard.

macOS 10.12.2+

``` source
@MainActor
init(coder: NSCoder)
```

## Return Value

A properly initialized scrubber selection style object.

## See Also

### Creating a selection style

init()

Initializes a new scrubber selection style.

func makeSelectionView() -> NSScrubberSelectionView?

Provides an opportunity to create a customized scrubber selection style.

