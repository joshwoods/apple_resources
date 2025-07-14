

- Core NFC
- NFCNDEFPayload
-  wellKnowTypeTextPayload(string:locale:) Deprecated

Type Method

# wellKnowTypeTextPayload(string:locale:)

Creates a payload record with text.

iOS 13.0–13.0DeprecatediPadOS 13.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class func wellKnowTypeTextPayload(
    string text: String,
    locale: Locale
) -> Self?
```

## Return Value

An NDEF payload record.

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

init(format: NFCTypeNameFormat, type: Data, identifier: Data, payload: Data, chunkSize: Int)

Creates a payload record with the specified format, type, identifier, payload data, and data chunk size.

