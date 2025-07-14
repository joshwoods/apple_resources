

- Core NFC
- NFCTypeNameFormat
-  NFCTypeNameFormat.unchanged 

Case

# NFCTypeNameFormat.unchanged

A type indicating that the payload is part of a series of records containing chunked data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
case unchanged
```

## Discussion

The first record in a series of chunked data records indicates the type name format for the series. The remaining records have a type name format of NFCTypeNameFormat.unchanged.

## See Also

### Content Types

case absoluteURI

A type indicating that the payload contains a uniform resource identifier.

case empty

A type indicating that the payload contains no data.

case media

A type indicating that the payload contains media data as defined by RFC 2046.

case nfcExternal

A type indicating that the payload contains NFC external type data.

case nfcWellKnown

A type indicating that the payload contains well-known NFC record type data.

case unknown

A type indicating that the payload data type is unknown.

