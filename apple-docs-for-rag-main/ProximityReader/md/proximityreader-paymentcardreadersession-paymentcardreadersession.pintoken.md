

- ProximityReader
- PaymentCardReaderSession
-  PaymentCardReaderSession.PINToken 

Structure

# PaymentCardReaderSession.PINToken

A secure PIN token that you receive from your participating payment service provider.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+

``` source
struct PINToken
```

## Mentioned in 

Adding support for Tap to Pay on iPhone to your app

## Overview

When the payment card issuer requests the PIN during a transaction, your participating payment service provider must provide this token as part of the response.

## Topics

### Creating a token

init(rawValue: String)

Creates a token with the string your payment service provider gave you.

### Getting the token value

let rawValue: String

The raw token string from your payment service provider.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Requesting the PIN

func capturePIN(using: PaymentCardReaderSession.PINToken, cardReaderTransactionID: String) async throws -> PaymentCardReadResult

Presents a sheet to capture the PIN when required by the payment card issuer, and returns the previously encrypted card data including newly captured PIN data.

