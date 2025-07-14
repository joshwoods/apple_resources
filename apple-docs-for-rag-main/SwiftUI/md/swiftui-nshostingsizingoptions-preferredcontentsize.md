

- SwiftUI
- NSHostingSizingOptions
-  preferredContentSize 

Type Property

# preferredContentSize

The hosting controller creates and updates constraints that represent its content’s ideal size. These constraints in turn influence the hosting controller’s `preferredContentSize`.

macOS 13.0+

``` source
static let preferredContentSize: NSHostingSizingOptions
```

## Discussion

The constraints reflect the size that fits a proposal of `.unspecified`.

Note

This option has no effect when used with an `NSHostingView` directly.

## See Also

### Geting sizing options

static let intrinsicContentSize: NSHostingSizingOptions

The hosting view creates and updates constraints that represent its content’s ideal size. These constraints in turn influence the hosting view’s `intrinsicContentSize`.

static let maxSize: NSHostingSizingOptions

The hosting view creates and updates constraints that represent its content’s maximum size.

static let minSize: NSHostingSizingOptions

The hosting view creates and updates constraints that represent its content’s minimum size.

static let standardBounds: NSHostingSizingOptions

The hosting view creates constraints for its minimum, ideal, and maximum sizes.

