

- SwiftUI
-  UIHostingControllerSizingOptions 

Structure

# UIHostingControllerSizingOptions

Options for how a hosting controller tracks its content’s size.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
struct UIHostingControllerSizingOptions
```

## Topics

### Getting sizing options

static let intrinsicContentSize: UIHostingControllerSizingOptions

The hosting controller’s view automatically invalidate its intrinsic content size when its ideal size changes.

static let preferredContentSize: UIHostingControllerSizingOptions

The hosting controller tracks its content’s ideal size in its preferred content size.

### Creating a sizing option

init(rawValue: Int)

Creates a new option set from a raw value.

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

### Displaying SwiftUI views in UIKit

Using SwiftUI with UIKit

Learn how to incorporate SwiftUI views into a UIKit app.

Unifying your app’s animations

Create a consistent UI animation experience across SwiftUI, UIKit, and AppKit.

class UIHostingController

A UIKit view controller that manages a SwiftUI view hierarchy.

struct UIHostingConfiguration

A content configuration suitable for hosting a hierarchy of SwiftUI views.

