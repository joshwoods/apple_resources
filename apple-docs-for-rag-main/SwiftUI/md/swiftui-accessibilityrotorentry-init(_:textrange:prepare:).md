

- SwiftUI
- AccessibilityRotorEntry
-  init(\_:textRange:prepare:) 

Initializer

# init(\_:textRange:prepare:)

Create a Rotor entry with a specific label and range. This Rotor entry will be associated with the Accessibility element that owns the Rotor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ label: Text? = nil,
    textRange: Range,
    prepare: @escaping () -> Void = {}
) where ID == Never
```

Show all declarations

## Parameters 

`label`  

Optional localized string used to show this Rotor entry to users. If no label is specified, the Rotor entry will be labeled based on the text at that range.

`prepare`  

Optional closure to run before a Rotor entry is navigated to, to prepare the UI as needed. This can be used to bring the UI element or text on-screen if it isn’t already, and SwiftUI not able to automatically scroll to it.

## See Also

### Creating a rotor entry

init(_:id:textRange:prepare:)

Create a Rotor entry with a specific label and identifier, with an optional range.

