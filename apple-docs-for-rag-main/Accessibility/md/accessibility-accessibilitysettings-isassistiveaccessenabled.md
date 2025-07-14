

- Accessibility
- AccessibilitySettings
-  isAssistiveAccessEnabled 

Type Property

# isAssistiveAccessEnabled

A Boolean value that indicates whether Assistive Access is running.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static var isAssistiveAccessEnabled: Bool { get }
```

## Mentioned in 

Optimizing your app for Assistive Access

## Discussion

The value of this property doesn’t change during a process’s lifetime, so it isn’t necessary to observe changes.

## See Also

### Related Documentation

var accessibilityAssistiveAccessEnabled: Bool { get }

A Boolean value that indicates whether Assistive Access is in use.

### Supporting cognitive accessibility features

Assistive Access

A mode that tailors the iOS and iPadOS experience for people with cognitive disabilities.

UISupportsFullScreenInAssistiveAccess

A Boolean value that indicates if an iOS or iPadOS app appears as full screen in Assistive Access.

