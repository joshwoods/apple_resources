

- LiveCommunicationKit
- Handle
-  init(type:value:displayName:) 

Initializer

# init(type:value:displayName:)

Creates a new `Handle`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
init(
    type: Handle.Kind,
    value: String,
    displayName: String? = nil
)
```

## Parameters 

`type`  

The type of handle (e.g. a phone number or email address)

`value`  

The raw value of the handle.

`displayName`  

The value that should be displayed to the user at the UI layer. If the given `displayName` is `nil` then the `value` is used instead.

