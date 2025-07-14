

- FinanceKit
-  AuthorizationStatus 

Enumeration

# AuthorizationStatus

iOS 17.4+iPadOS 17.4+

``` source
enum AuthorizationStatus
```

## Topics

### Operators

static func == (AuthorizationStatus, AuthorizationStatus) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case authorized

A person authorized the app to use FinanceKit services.

case denied

A person denied the use of FinanceKit services for the app

case notDetermined

A person has not chosen whether the app can use FinanceKit services.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Authorization

func authorizationStatus() async throws -> AuthorizationStatus

Checks the authorization status for the calling application.

func requestAuthorization() async throws -> AuthorizationStatus

Prompts a person to give FinanceKit authorization to access financial data.

