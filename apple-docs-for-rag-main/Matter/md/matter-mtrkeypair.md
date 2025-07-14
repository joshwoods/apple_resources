

- Matter
-  MTRKeypair 

Protocol

# MTRKeypair

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
protocol MTRKeypair : NSObjectProtocol
```

## Mentioned in 

Onboarding a Matter device

## Topics

### Instance Methods

func publicKey() -> Unmanaged&lt;SecKey>Deprecated

func signMessageECDSA_DER(Data) -> Data

func signMessageECDSA_RAW(Data) -> Data

func copyPublicKey() -> SecKey

## Relationships

### Inherits From

- NSObjectProtocol

