

- SwiftUI
- FocusInteractions
-  activate 

Type Property

# activate

The view has a primary action that can be activated via focus gestures.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static let activate: FocusInteractions
```

## Discussion

On macOS and iOS, focus-driven activation interactions are only possible when all-controls keyboard navigation is enabled. On tvOS and watchOS, focus-driven activation interactions are always possible.

## See Also

### Creating the interaction types

static var automatic: FocusInteractions

The view supports whatever focus-driven interactions are commonly expected for interactive content on the current platform.

static let edit: FocusInteractions

The view captures input from non-spatial sources like a keyboard or Digital Crown.

