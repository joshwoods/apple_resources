

- Authentication Services
- ASCredentialServiceIdentifier
-  ASCredentialServiceIdentifier.IdentifierType 

Enumeration

# ASCredentialServiceIdentifier.IdentifierType

Possible values for the service identifier type.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
enum IdentifierType
```

## Topics

### Identifier types

case URL

A URL service identifier.

case domain

A domain service identifier.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Identifying the credential service

var identifier: String

A string that names the identified service.

var type: ASCredentialServiceIdentifier.IdentifierType

The kind of services that the identifier represents.

