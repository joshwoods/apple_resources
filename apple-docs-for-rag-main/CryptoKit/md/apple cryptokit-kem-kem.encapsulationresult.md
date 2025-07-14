

- Apple CryptoKit
- KEM
-  KEM.EncapsulationResult 

Structure

# KEM.EncapsulationResult

The result of an encapsulation operation

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct EncapsulationResult
```

## Topics

### Initializers

init(sharedSecret: SymmetricKey, encapsulated: Data)

### Instance Properties

let encapsulated: Data

The encapsulated secret

let sharedSecret: SymmetricKey

The shared secret

## Relationships

### Conforms To

- Sendable

