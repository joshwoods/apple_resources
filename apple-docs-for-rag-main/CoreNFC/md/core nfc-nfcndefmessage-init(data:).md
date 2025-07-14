

- Core NFC
- NFCNDEFMessage
-  init(data:) 

Initializer

# init(data:)

Creates an NDEF message from raw data representing the message.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
convenience init?(data: Data)
```

## Parameters 

`data`  

A data object containing the raw bytes of a complete NDEF message. The data must contain only one NDEF message, and the message must contain NDEF payloads that are valid according to the NFC Forum NDEF RTD specification.

## Return Value

An NDEF message, or `nil` when the raw data is invalid.

## See Also

### Creating an NDEF Message

init(records: [NFCNDEFPayload])

Creates an NDEF message with the specified records.

