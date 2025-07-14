

- SwiftUI
- NSHostingSizingOptions
-  maxSize 

Type Property

# maxSize

The hosting view creates and updates constraints that represent its content’s maximum size.

macOS 13.0+

``` source
static let maxSize: NSHostingSizingOptions
```

## Discussion

The constraints reflect the size that fits a proposal of `width: infinity, height: infinity`.

## See Also

### Geting sizing options

static let intrinsicContentSize: NSHostingSizingOptions

The hosting view creates and updates constraints that represent its content’s ideal size. These constraints in turn influence the hosting view’s `intrinsicContentSize`.

static let minSize: NSHostingSizingOptions

The hosting view creates and updates constraints that represent its content’s minimum size.

static let preferredContentSize: NSHostingSizingOptions

The hosting controller creates and updates constraints that represent its content’s ideal size. These constraints in turn influence the hosting controller’s `preferredContentSize`.

static let standardBounds: NSHostingSizingOptions

The hosting view creates constraints for its minimum, ideal, and maximum sizes.

