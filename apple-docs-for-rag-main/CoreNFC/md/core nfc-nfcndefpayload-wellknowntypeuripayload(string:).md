

- Core NFC
- NFCNDEFPayload
-  wellKnownTypeURIPayload(string:) 

Type Method

# wellKnownTypeURIPayload(string:)

Creates a payload record with a URI specified as a string.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class func wellKnownTypeURIPayload(string uri: String) -> Self?
```

## Parameters 

`uri`  

A URL string.

## Return Value

An NDEF payload record.

## Discussion

Use this method to create NDEF URI payload records that you can’t create using a URL object, such as a URI containing special characters not represented by 7-bit ASCII encoding such as ä and ö.

## See Also

### Creating a Payload Record

class func wellKnownTypeURIPayload(url: URL) -> Self?

Creates a payload record with a URI specified as a URL.

class func wellKnownTypeTextPayload(string: String, locale: Locale) -> Self?

Creates a payload record with text.

init(format: NFCTypeNameFormat, type: Data, identifier: Data, payload: Data)

Creates a payload record with the specified format, type, identifier, and payload data.

init(format: NFCTypeNameFormat, type: Data, identifier: Data, payload: Data, chunkSize: Int)

Creates a payload record with the specified format, type, identifier, payload data, and data chunk size.

class func wellKnowTypeTextPayload(string: String, locale: Locale) -> Self?

Creates a payload record with text.

Deprecated

