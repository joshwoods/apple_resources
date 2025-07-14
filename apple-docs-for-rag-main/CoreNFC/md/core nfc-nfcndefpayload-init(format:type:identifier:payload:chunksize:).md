

- Core NFC
- NFCNDEFPayload
-  init(format:type:identifier:payload:chunkSize:) 

Initializer

# init(format:type:identifier:payload:chunkSize:)

Creates a payload record with the specified format, type, identifier, payload data, and data chunk size.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
init(
    format: NFCTypeNameFormat,
    type: Data,
    identifier: Data,
    payload: Data,
    chunkSize: Int
)
```

## Parameters 

`format`  

A NFC type name format value.

`type`  

A data object describing the type of payload. If the data is empty, the method excludes this field from the payload record.

`identifier`  

A URI reference that identifies the payload. If the data is empty, the method excludes this field from the payload record.

`payload`  

A data object containing the payload data. If the data is empty, the method excludes this field from the payload record.

`chunkSize`  

The maximum size of a payload chunk. A value of zero indicates that the payload fits in a single record, that is, no chunking of the payload.

## Return Value

A newly initialized payload record object.

## See Also

### Creating a Payload Record

class func wellKnownTypeURIPayload(url: URL) -> Self?

Creates a payload record with a URI specified as a URL.

class func wellKnownTypeURIPayload(string: String) -> Self?

Creates a payload record with a URI specified as a string.

class func wellKnownTypeTextPayload(string: String, locale: Locale) -> Self?

Creates a payload record with text.

init(format: NFCTypeNameFormat, type: Data, identifier: Data, payload: Data)

Creates a payload record with the specified format, type, identifier, and payload data.

class func wellKnowTypeTextPayload(string: String, locale: Locale) -> Self?

Creates a payload record with text.

Deprecated

