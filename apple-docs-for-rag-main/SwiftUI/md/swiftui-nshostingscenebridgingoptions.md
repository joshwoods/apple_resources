

- SwiftUI
-  NSHostingSceneBridgingOptions 

Structure

# NSHostingSceneBridgingOptions

Options for how hosting views and controllers manage aspects of the associated window.

macOS 14.0+

``` source
struct NSHostingSceneBridgingOptions
```

## Topics

### Geting bridging options

static let all: NSHostingSceneBridgingOptions

The hosting view’s associated window will have both its title bars and toolbars populated with values from their respective modifiers.

static let title: NSHostingSceneBridgingOptions

The hosting view’s associated window will have its title and subtitle populated with the values provided to the `navigationTitle(_:)` and `navigationSubtitle(_:)` modifiers, respectively.

static let toolbars: NSHostingSceneBridgingOptions

The hosting view’s associated window will have its toolbar populated with any items provided to the `toolbar(content:)` modifier.

### Creating a bridging options

init(rawValue: Int)

Creates a new set from a raw value.

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

struct NSHostingSizingOptions

Options for how hosting views and controllers reflect their content’s size into Auto Layout constraints.

