

- Group Activities
- CustomMessageIdentifiable
-  messageIdentifier 

Type Property

# messageIdentifier

A custom identification string for the current type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static var messageIdentifier: String { get }
```

**Required**

## Discussion

The string you return from this property must be unique among your app’s custom message types. When you send a message, GroupSessionMessenger includes this string in the data it sends to other devices. When it receives a message, GroupSessionMessenger creates the type that contains the matching string in this property.

