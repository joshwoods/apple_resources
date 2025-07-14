

- Objective-C Runtime
- NSObject
-  accessibilityElementDidBecomeFocused() 

Instance Method

# accessibilityElementDidBecomeFocused()

Sent after an assistive technology has set its virtual focus on the accessibility element.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func accessibilityElementDidBecomeFocused()
```

## Discussion

Override `accessibilityElementDidBecomeFocused` if you need to know when an assistive technology has set its virtual focus on an accessibility element.

## See Also

### Getting focus information

func accessibilityElementDidLoseFocus()

Sent after an assistive technology has removed its virtual focus from an accessibility element.

func accessibilityElementIsFocused() -> Bool

Returns a Boolean value indicating whether an assistive technology is focused on the accessibility element.

func accessibilityAssistiveTechnologyFocusedIdentifiers() -> Set&lt;UIAccessibility.AssistiveTechnologyIdentifier>?

Returns a set of identifier keys indicating which assistive app has focus on the accessibility element.

