

- SwiftUI
- NSHostingSizingOptions
-  minSize 

Type Property

# minSize

The hosting view creates and updates constraints that represent its content’s minimum size.

macOS 13.0+

``` source
static let minSize: NSHostingSizingOptions
```

## Discussion

The constraints reflect the size that fits a proposal of `width: 0, height: 0`.

## See Also

### Geting sizing options

static let intrinsicContentSize: NSHostingSizingOptions

The hosting view creates and updates constraints that represent its content’s ideal size. These constraints in turn influence the hosting view’s `intrinsicContentSize`.

static let maxSize: NSHostingSizingOptions

The hosting view creates and updates constraints that represent its content’s maximum size.

static let preferredContentSize: NSHostingSizingOptions

The hosting controller creates and updates constraints that represent its content’s ideal size. These constraints in turn influence the hosting controller’s `preferredContentSize`.

static let standardBounds: NSHostingSizingOptions

The hosting view creates constraints for its minimum, ideal, and maximum sizes.

