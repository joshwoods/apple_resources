

- PassKit (Apple Pay and Wallet)
-  PKIdentityElement 

Class

# PKIdentityElement

An object that represents the elements an app requests from identity documents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class PKIdentityElement
```

## Overview

If an app requests an element from a document type that doesn’t support it, the system ignores the element.

## Topics

### Getting identity elements

class var address: PKIdentityElement

An element that represents the user’s home address.

class var dateOfBirth: PKIdentityElement

An element that represents the user’s date of birth.

class var documentIssueDate: PKIdentityElement

An element that represents the issue date of the document.

class var documentExpirationDate: PKIdentityElement

An element that represents the expiration date of the document.

class var documentNumber: PKIdentityElement

An element that represents the document’s number, as the issuing authority defines.

class var drivingPrivileges: PKIdentityElement

An element that represents the user’s driving privileges.

class var familyName: PKIdentityElement

An element that represents the user’s family name.

class var givenName: PKIdentityElement

An element that represents the user’s given name.

class var issuingAuthority: PKIdentityElement

An element that represents the user’s issuing authority.

class var portrait: PKIdentityElement

An element that represents the user’s photo.

### Getting an age identity element

class var age: PKIdentityElement

An element that represents the user’s age, in years.

class func age(atLeast: Int) -> Self

Returns an element that represents the user’s age is at least the age you specify.

### Type Properties

class var documentDHSComplianceStatus: PKIdentityElement

class var sex: PKIdentityElement

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Identity sheet interactions and authorization

Requesting identity data from a Wallet pass

Initiate a request for identity information by prompting a user for permission and decrypting a response payload.

Verifying Wallet identity requests

Decrypt and verify an in-app presentment request on your server.

class PKIdentityAuthorizationController

An object that presents a sheet that prompts the user to allow a request for identity information.

class PKIdentityRequest

An object that represents a request for identity information from a Wallet pass.

class PKIdentityDocument

An object that represents the response to a request.

class PKIdentityButton

An object that displays a button to trigger the identity verification flow.

struct VerifyIdentityWithWalletButton

A view that displays a button for identity verification.

struct VerifyIdentityWithWalletButtonLabel

A type that represents the label you use with a verify identity button.

struct VerifyIdentityWithWalletButtonStyle

A type that represents the style you use with a verify identity button.

