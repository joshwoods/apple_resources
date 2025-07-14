

- Apple CryptoKit
-  KEMPrivateKey 

Protocol

# KEMPrivateKey

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@preconcurrency
protocol KEMPrivateKey : Sendable
```

## Topics

### Associated Types

associatedtype PublicKey : KEMPublicKey

**Required**

### Instance Properties

var publicKey: Self.PublicKey

Returns the associated public key

**Required**

### Instance Methods

func decapsulate(Data) throws -> SymmetricKey

Decapsulates the encapsulated shared secret

**Required**

### Type Methods

static func generate() throws -> Self

Generate a new random Private Key

**Required**

## Relationships

### Inherits From

- Sendable

