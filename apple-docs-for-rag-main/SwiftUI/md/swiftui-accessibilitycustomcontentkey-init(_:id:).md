

- SwiftUI
- AccessibilityCustomContentKey
-  init(\_:id:) 

Initializer

# init(\_:id:)

Create an `AccessibilityCustomContentKey` with the specified label and identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ label: Text,
    id: String
)
```

Show all declarations

## Parameters 

`label`  

Localized text describing to the user what is contained in this additional information entry. For example: “orientation”.

`id`  

String used to identify the additional information entry to SwiftUI. Adding an entry will replace any previous value with the same identifier.

## See Also

### Creating a key

init(LocalizedStringKey)

Create an `AccessibilityCustomContentKey` with the specified label.

