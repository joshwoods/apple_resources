

- Security
-  SecKeyKeyExchangeParameter 

Structure

# SecKeyKeyExchangeParameter

The dictionary keys used to specify Diffie-Hellman key exchange parameters.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
struct SecKeyKeyExchangeParameter
```

## Discussion

Use these constants as keys in the dictionary that you input to the SecKeyCopyKeyExchangeResult(_:_:_:_:_:) function as a means to refine the process of Diffie-Hellman key exchange.

## Topics

### Type Properties

static let requestedSize: SecKeyKeyExchangeParameter

static let sharedInfo: SecKeyKeyExchangeParameter

### Initializers

init(rawValue: CFString)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

