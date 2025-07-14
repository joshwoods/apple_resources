

- Core NFC
- NFCNDEFPayload
-  wellKnownTypeURIPayload(url:) 

Type Method

# wellKnownTypeURIPayload(url:)

Creates a payload record with a URI specified as a URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class func wellKnownTypeURIPayload(url: URL) -> Self?
```

## Parameters 

`url`  

A URL object.

## Return Value

An NDEF payload record.

## See Also

### Creating a Payload Record

class func wellKnownTypeURIPayload(string: String) -> Self?

Creates a payload record with a URI specified as a string.

class func wellKnownTypeTextPayload(string: String, locale: Locale) -> Self?

Creates a payload record with text.

init(format: NFCTypeNameFormat, type: Data, identifier: Data, payload: Data)

Creates a payload record with the specified format, type, identifier, and payload data.

init(format: NFCTypeNameFormat, type: Data, identifier: Data, payload: Data, chunkSize: Int)

Creates a payload record with the specified format, type, identifier, payload data, and data chunk size.

class func wellKnowTypeTextPayload(string: String, locale: Locale) -> Self?

Creates a payload record with text.

Deprecated

