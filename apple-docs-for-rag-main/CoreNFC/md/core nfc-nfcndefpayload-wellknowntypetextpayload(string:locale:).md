

- Core NFC
- NFCNDEFPayload
-  wellKnownTypeTextPayload(string:locale:) 

Type Method

# wellKnownTypeTextPayload(string:locale:)

Creates a payload record with text.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class func wellKnownTypeTextPayload(
    string text: String,
    locale: Locale
) -> Self?
```

## Parameters 

`text`  

Text to include in the payload.

`locale`  

A locale object. This method saves the IANA language code, specified by the locale, to the payload.

## Return Value

An NDEF payload record.

## See Also

### Creating a Payload Record

class func wellKnownTypeURIPayload(url: URL) -> Self?

Creates a payload record with a URI specified as a URL.

class func wellKnownTypeURIPayload(string: String) -> Self?

Creates a payload record with a URI specified as a string.

init(format: NFCTypeNameFormat, type: Data, identifier: Data, payload: Data)

Creates a payload record with the specified format, type, identifier, and payload data.

init(format: NFCTypeNameFormat, type: Data, identifier: Data, payload: Data, chunkSize: Int)

Creates a payload record with the specified format, type, identifier, payload data, and data chunk size.

class func wellKnowTypeTextPayload(string: String, locale: Locale) -> Self?

Creates a payload record with text.

Deprecated

