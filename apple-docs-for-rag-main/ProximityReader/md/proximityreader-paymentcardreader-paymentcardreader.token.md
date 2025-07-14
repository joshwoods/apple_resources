

- ProximityReader
- PaymentCardReader
-  PaymentCardReader.Token 

Structure

# PaymentCardReader.Token

A secure token that you receive from your participating payment service provider.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
struct Token
```

## Overview

You must create a secure token to use Tap to Pay on iPhone. Your payment service provider supplies the string you use to create this token. Create your token and pass it to the prepare(using:) method to configure the current device to read cards.

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

### Displaying the Tap to Pay on iPhone’s terms and conditions

func isAccountLinked(using: PaymentCardReader.Token) async throws -> Bool

A Boolean value that indicates whether the account is already linked.

func linkAccount(using: PaymentCardReader.Token) async throws

Presents a sheet for the merchant to accept Tap to Pay on iPhone’s Terms and Conditions on a device.

func relinkAccount(using: PaymentCardReader.Token) async throws

Presents a sheet for the merchant to re-accept Tap to Pay on iPhone’s Terms and Conditions on a device using a different Apple Account.

