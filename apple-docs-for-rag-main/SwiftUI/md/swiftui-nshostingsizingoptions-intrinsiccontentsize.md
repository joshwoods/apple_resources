

- SwiftUI
- NSHostingSizingOptions
-  intrinsicContentSize 

Type Property

# intrinsicContentSize

The hosting view creates and updates constraints that represent its content’s ideal size. These constraints in turn influence the hosting view’s `intrinsicContentSize`.

macOS 13.0+

``` source
static let intrinsicContentSize: NSHostingSizingOptions
```

## Discussion

The constraints reflect the size that fits a proposal of `.unspecified`.

## See Also

### Geting sizing options

static let maxSize: NSHostingSizingOptions

The hosting view creates and updates constraints that represent its content’s maximum size.

static let minSize: NSHostingSizingOptions

The hosting view creates and updates constraints that represent its content’s minimum size.

static let preferredContentSize: NSHostingSizingOptions

The hosting controller creates and updates constraints that represent its content’s ideal size. These constraints in turn influence the hosting controller’s `preferredContentSize`.

static let standardBounds: NSHostingSizingOptions

The hosting view creates constraints for its minimum, ideal, and maximum sizes.

