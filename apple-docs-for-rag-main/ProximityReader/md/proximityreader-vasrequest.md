

- ProximityReader
-  VASRequest 

Class

# VASRequest

A request to read a contactless loyalty card and retrieve loyalty program identifiers for the person.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
class VASRequest
```

## Mentioned in 

Accepting loyalty passes from Wallet

## Overview

Create a `VASRequest` object to obtain details from someone’s loyalty card so that you can process associated transactions. After you create this object, pass it to the readVAS(_:)or readPaymentCard(_:vasRequest:stopOnVASResult:) method of PaymentCardReaderSession.

## Topics

### Creating a loyalty card request

init(vasMerchants: [VASRequest.Merchant], localizedVASType: String)

Creates a request to read loyalty card service information.

### Getting the loyalty card details

let localizedVASType: String

The localized name of the loyalty program.

let vasMerchants: [VASRequest.Merchant]

The list of merchants to match against the user’s Wallet content or loyalty card.

struct Merchant

The identity of a merchant that offers a loyalty program.

### Setting the user interface language

var userInterfaceLanguage: Locale.Language?

The language to use when localizing the user interface.

## Relationships

### Conforms To

- Sendable

## See Also

### Loyalty card requests

Accepting loyalty passes from Wallet

Set up the necessary components so your app can begin using Tap to Pay on iPhone to read and issue loyalty passes.

struct VASReadResult

The result of a request to read loyalty card information.

