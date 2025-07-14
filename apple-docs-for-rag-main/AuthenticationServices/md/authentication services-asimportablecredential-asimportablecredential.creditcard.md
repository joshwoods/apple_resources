

- Authentication Services
- ASImportableCredential
-  ASImportableCredential.CreditCard 

Structure

# ASImportableCredential.CreditCard

A type to represent credit card information.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
struct CreditCard
```

## Overview

This type is a representation of `CreditCard` as defined in the Credential Exchange Format (CXF) specification.

## Topics

### Creating a credit card instance

init(number: String, fullName: String, cardType: String?, verificationNumber: String?, expiryDate: String?, validFrom: String?)

Creates a credit card instance.

### Accessing credit card properties

var number: String

The card number.

var fullName: String

The full name of the card owner.

var cardType: String?

The card type, if any.

var verificationNumber: String?

The verification number, such as the CVC code.

var expiryDate: String?

The expiration date, if any, in MM/DD format.

var validFrom: String?

The date from which the card is valid, if any.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Identity credential types

case creditCard(ASImportableCredential.CreditCard)

A credit card credential.

