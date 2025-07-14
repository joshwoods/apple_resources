

- CryptoTokenKit
-  TKTokenKeyAlgorithm 

Class

# TKTokenKeyAlgorithm

Cryptographic algorithms used by token keys.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKTokenKeyAlgorithm
```

## Overview

Typically, the supported algorithm for a token key can be represented by a value of the `SecKeyAlgorithm` enumeration. However, tokens such as Smart Cards require that input data for operations take the format of a more specific algorithm. For example, a token may accept raw data to generate a cryptographic signature, but require that raw data to be formatted according to PKCS1 padding rules. To express such a requirement, a `TKTokenKeyAlgorithm` object defines a target algorithm and a set of other algorithms that were used. In the previous example, the target algorithm is `kSecKeyAlgorithmRSASignatureRaw` and the `kSecKeyAlgorithmRSASignatureDigestPKCS1v15SHA1` algorithm is also reported as being used.

## Topics

### Determining Algorithm Usage

func isAlgorithm(SecKeyAlgorithm) -> Bool

Returns whether the specified algorithm is the target operation algorithm.

func supportsAlgorithm(SecKeyAlgorithm) -> Bool

Whether the specified algorithm is the target operation algorithm, or one of the other algorithms used.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Determining Support for Operations

func tokenSession(TKTokenSession, supports: TKTokenOperation, keyObjectID: TKToken.ObjectID, algorithm: TKTokenKeyAlgorithm) -> Bool

Asks the delegate whether the token session supports a given operation using the specified key and algorithm.

enum TKTokenOperation

Operations that can be performed with a token’s keys and certificates.

typealias ObjectID

A unique and persistent identifier of a particular token object.

