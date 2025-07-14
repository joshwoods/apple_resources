

- Objective-C Runtime
- NSObject
-  accessibilityElementIsFocused() 

Instance Method

# accessibilityElementIsFocused()

Returns a Boolean value indicating whether an assistive technology is focused on the accessibility element.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func accessibilityElementIsFocused() -> Bool
```

## Return Value

YES if an assistive technology is virtually focused on the element; otherwise, NO.

## See Also

### Getting focus information

func accessibilityElementDidBecomeFocused()

Sent after an assistive technology has set its virtual focus on the accessibility element.

func accessibilityElementDidLoseFocus()

Sent after an assistive technology has removed its virtual focus from an accessibility element.

func accessibilityAssistiveTechnologyFocusedIdentifiers() -> Set&lt;UIAccessibility.AssistiveTechnologyIdentifier>?

Returns a set of identifier keys indicating which assistive app has focus on the accessibility element.

