

- Apple Pay Merchant Token Management API
-  MerchantTokenMetadata 

Object

# MerchantTokenMetadata

The card information related to a merchant token, including its card art and metadata.

App Store Connect API 1.0.10+

``` source
object MerchantTokenMetadata
```

## Properties

`cardArt`

`[`CardArt`]`

An array that contains data you use to display art that represents the card related to the merchant token.

`cardMetadata`

CardMetadata

Card data, including its expiration date and suffix, for the card related to the merchant token.

## See Also

### Merchant token event retrieval

Get Details of a Merchant Token Event

Get the details of a merchant token event after receiving a notification.

object MerchantTokenEventResponse

A response body that contains information about a life-cycle event for a merchant token.

object CardArt

Data for displaying art to represent a card.

object CardMetadata

Data about the card, including its expiration date and suffix.

