

- Objective-C Runtime
- NSObject
-  accessibilityAssistiveTechnologyFocusedIdentifiers() 

Instance Method

# accessibilityAssistiveTechnologyFocusedIdentifiers()

Returns a set of identifier keys indicating which assistive app has focus on the accessibility element.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func accessibilityAssistiveTechnologyFocusedIdentifiers() -> Set?
```

## See Also

### Getting focus information

func accessibilityElementDidBecomeFocused()

Sent after an assistive technology has set its virtual focus on the accessibility element.

func accessibilityElementDidLoseFocus()

Sent after an assistive technology has removed its virtual focus from an accessibility element.

func accessibilityElementIsFocused() -> Bool

Returns a Boolean value indicating whether an assistive technology is focused on the accessibility element.

