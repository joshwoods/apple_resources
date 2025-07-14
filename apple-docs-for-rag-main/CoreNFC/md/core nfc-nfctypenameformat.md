

- Core NFC
-  NFCTypeNameFormat 

Enumeration

# NFCTypeNameFormat

The Type Name Format values that specify the content type for the payload data in an NFC NDEF message.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
enum NFCTypeNameFormat
```

## Topics

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

case unchanged

A type indicating that the payload is part of a series of records containing chunked data.

case unknown

A type indicating that the payload data type is unknown.

### Initializers

init?(rawValue: UInt8)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Information About a Payload Record

var identifier: Data

The identifier of the payload, as defined by the NDEF specification.

var payload: Data

The payload, as defined by the NDEF specification.

var type: Data

The type of the payload, as defined by the NDEF specification.

var typeNameFormat: NFCTypeNameFormat

The Type Name Format field of the payload, as defined by the NDEF specification.

