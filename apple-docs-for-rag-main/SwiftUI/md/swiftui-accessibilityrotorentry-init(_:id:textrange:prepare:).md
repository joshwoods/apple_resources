

- SwiftUI
- AccessibilityRotorEntry
-  init(\_:id:textRange:prepare:) 

Initializer

# init(\_:id:textRange:prepare:)

Create a Rotor entry with a specific label and identifier, with an optional range.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ label: Text,
    id: ID,
    textRange: Range? = nil,
    prepare: @escaping () -> Void = {}
)
```

Show all declarations

## Parameters 

`label`  

Localized string used to show this Rotor entry to users.

`id`  

Used to find the UI element associated with this Rotor entry. This identifier should be used within a `scrollView`, either in a `ForEach` or using an `id` call.

`textRange`  

Optional range of text associated with this Rotor entry. This should be a range within text that is set as the either label or accessibility value of the associated element.

`prepare`  

Optional closure to run before a Rotor entry is navigated to, to prepare the UI as needed. This can be used to bring the UI element on-screen if it isn’t already, and SwiftUI is not able to automatically scroll to it.

## See Also

### Creating a rotor entry

init(_:textRange:prepare:)

Create a Rotor entry with a specific label and range. This Rotor entry will be associated with the Accessibility element that owns the Rotor.

