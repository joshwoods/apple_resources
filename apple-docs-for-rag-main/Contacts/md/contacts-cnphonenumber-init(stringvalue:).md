

- Contacts
- CNPhoneNumber
-  init(stringValue:) 

Initializer

# init(stringValue:)

Returns a new phone number object initialized with the specified phone number string.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
init(stringValue string: String)
```

## Parameters 

`string`  

A string value with which to initializes the phone number object.

## Return Value

A newly initialized phone number object.

## Discussion

You should initialize this with a phone number string. This method returns `nil` when the value of `string` is `nil`.

