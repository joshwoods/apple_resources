

- AppKit
- NSScrubberSelectionStyle
-  makeSelectionView() 

Instance Method

# makeSelectionView()

Provides an opportunity to create a customized scrubber selection style.

macOS 10.12.2+

``` source
@MainActor
func makeSelectionView() -> NSScrubberSelectionView?
```

## Return Value

A correctly configured scrubber selection view that represents the appearance of your custom selection style.

## Discussion

In an NSScrubberSelectionStyle subclass that you create, override this method to create a custom selection style.

## See Also

### Creating a selection style

init()

Initializes a new scrubber selection style.

init(coder: NSCoder)

Initializes a scrubber selection style when included from a nib or Storyboard.

