

- SwiftUI
- EnvironmentValues
-  isScrollEnabled 

Instance Property

# isScrollEnabled

A Boolean value that indicates whether any scroll views associated with this environment allow scrolling to occur.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var isScrollEnabled: Bool { get set }
```

## Discussion

The default value is `true`. Use the scrollDisabled(_:) modifier to configure this property.

## See Also

### Disabling scrolling

func scrollDisabled(Bool) -> some View

Disables or enables scrolling in scrollable views.

