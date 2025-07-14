

- SwiftUI
-  NSHostingSizingOptions 

Structure

# NSHostingSizingOptions

Options for how hosting views and controllers reflect their content’s size into Auto Layout constraints.

macOS 13.0+

``` source
struct NSHostingSizingOptions
```

## Topics

### Geting sizing options

static let intrinsicContentSize: NSHostingSizingOptions

The hosting view creates and updates constraints that represent its content’s ideal size. These constraints in turn influence the hosting view’s `intrinsicContentSize`.

static let maxSize: NSHostingSizingOptions

The hosting view creates and updates constraints that represent its content’s maximum size.

static let minSize: NSHostingSizingOptions

The hosting view creates and updates constraints that represent its content’s minimum size.

static let preferredContentSize: NSHostingSizingOptions

The hosting controller creates and updates constraints that represent its content’s ideal size. These constraints in turn influence the hosting controller’s `preferredContentSize`.

static let standardBounds: NSHostingSizingOptions

The hosting view creates constraints for its minimum, ideal, and maximum sizes.

### Creating a sizing option

init(rawValue: Int)

Creates a new options from a raw value.

let rawValue: Int

The raw value.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Displaying SwiftUI views in AppKit

Unifying your app’s animations

Create a consistent UI animation experience across SwiftUI, UIKit, and AppKit.

class NSHostingController

An AppKit view controller that hosts SwiftUI view hierarchy.

class NSHostingView

An AppKit view that hosts a SwiftUI view hierarchy.

class NSHostingMenu

An AppKit menu with menu items that are defined by a SwiftUI View.

struct NSHostingSceneBridgingOptions

Options for how hosting views and controllers manage aspects of the associated window.

