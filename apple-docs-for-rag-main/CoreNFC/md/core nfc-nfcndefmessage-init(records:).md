

- Core NFC
- NFCNDEFMessage
-  init(records:) 

Initializer

# init(records:)

Creates an NDEF message with the specified records.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
init(records: [NFCNDEFPayload])
```

## Parameters 

`records`  

An array of payload objects for the message. To create an empty message, pass in an empty array.

## Return Value

A newly initialized NDEF message object.

## See Also

### Creating an NDEF Message

convenience init?(data: Data)

Creates an NDEF message from raw data representing the message.

