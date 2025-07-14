

- ProximityReader
- VASRequest
-  VASRequest.Merchant 

Structure

# VASRequest.Merchant

The identity of a merchant that offers a loyalty program.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
struct Merchant
```

## Mentioned in 

Accepting loyalty passes from Wallet

## Overview

Create `Merchant` objects to identify merchants whose loyalty programs you support. When placing a request for loyalty card information, or Value Added Services (VAS) information, specify the associated merchant details. The system uses the merchant information to return details only for those merchants.

## Topics

### Creating a merchant structure

init(id: String, url: URL?, shouldSendURLOnly: Bool, localizedName: String?)

Creates a new merchant object with the specified information.

Deprecated

### Getting the merchant name

var localizedName: String

The localized name of the merchant or corresponding loyalty program.

### Getting the merchant URL details

let url: URL?

The URL to display to the customer if the matching loyalty or reward ID isn’t found.

let shouldSendURLOnly: Bool

A Boolean value that indicates whether to send only the merchant URL to the customer’s device without requesting data.

Deprecated

### Getting the merchant ID

let id: String

A unique identifier for the merchant.

### Initializers

init(id: String, url: URL?, localizedName: String?)

Creates a new merchant object with the specified information.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Identifiable
- Sendable

## See Also

### Getting the loyalty card details

let localizedVASType: String

The localized name of the loyalty program.

let vasMerchants: [VASRequest.Merchant]

The list of merchants to match against the user’s Wallet content or loyalty card.

