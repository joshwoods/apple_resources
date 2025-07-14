

- AdAttributionKit
-  AdAttributionKitError 

Enumeration

# AdAttributionKitError

Values that describe ad attribution error conditions.

iOS 17.4+iPadOS 17.4+Mac Catalyst

``` source
enum AdAttributionKitError
```

## Topics

### Operators

static func == (AdAttributionKitError, AdAttributionKitError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case conversionTagNotSupported

The postback update failed due to an unsupported use of conversion tag

case impressionExpired

The attribution failed because the impression expired.

case invalidConversionTag

The postback update failed due to an invalid conversion tag

case invalidImpressionJWSComponents

The attribution failed due to invalid JWS components.

case invalidImpressionJWSHeader

The attribution failed due to an invalid JWS header.

case invalidImpressionJWSPayload

The attribution failed due to an invalid JWS payload.

case invalidImpressionJWSSignature

The attribution failed due to an invalid JWS signature.

case missingAttributionView

The attribution failed due to a missing attribution view.

case unknown

The attribution failed due to an unknown, unrecoverable error.

### Instance Properties

var description: String

A string that describes the error.

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

Error Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Error
- Hashable
- Sendable

