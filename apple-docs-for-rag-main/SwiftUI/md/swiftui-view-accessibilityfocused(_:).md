

- SwiftUI
- View
-  accessibilityFocused(\_:) 

Instance Method

# accessibilityFocused(\_:)

Modifies this view by binding its accessibility element’s focus state to the given boolean state value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func accessibilityFocused(_ condition: AccessibilityFocusState.Binding) -> some View
```

## Parameters 

`condition`  

The accessibility focus state to bind. When accessibility focus moves to the accessibility element of the modified view, the focus value is set to `true`. If the value is set to `true` programmatically, then accessibility focus will move to accessibility element of the modified view. The value will be set to `false` if accessibility focus leaves the accessibility element of the modified view, and accessibility focus will be dismissed automatically if the value is set to `false` programmatically.

## Return Value

The modified view.

## See Also

### Controlling focus

func accessibilityFocused&lt;Value>(AccessibilityFocusState&lt;Value>.Binding, equals: Value) -> some View

Modifies this view by binding its accessibility element’s focus state to the given state value.

struct AccessibilityFocusState

A property wrapper type that can read and write a value that SwiftUI updates as the focus of any active accessibility technology, such as VoiceOver, changes.

