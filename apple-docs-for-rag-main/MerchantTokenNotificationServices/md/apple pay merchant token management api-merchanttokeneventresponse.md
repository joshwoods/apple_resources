

- Apple Pay Merchant Token Management API
-  MerchantTokenEventResponse 

Object

# MerchantTokenEventResponse

A response body that contains information about a life-cycle event for a merchant token.

App Store Connect API 1.0.10+

``` source
object MerchantTokenEventResponse
```

## Properties

`eventType`

`string`

 (Required) 

A field that indicates the type of event for this notification.

Maximum length: `64`

Possible Values: `UNLINK, UPDATED_METADATA, UPDATED_CARD_ART`

`merchantTokenIdentifier`

`string`

 (Required) 

The unique identifier of the merchant token.

Maximum length: `64`

`merchantTokenMetadata`

MerchantTokenMetadata

Data about the card, including its expiration date and suffix.

`reason`

`string`

 (Required) 

A string that indicates who originated the token event, either the user or the card issuer.

Maximum length: `256`

## See Also

### Merchant token event retrieval

Get Details of a Merchant Token Event

Get the details of a merchant token event after receiving a notification.

object MerchantTokenMetadata

The card information related to a merchant token, including its card art and metadata.

object CardArt

Data for displaying art to represent a card.

object CardMetadata

Data about the card, including its expiration date and suffix.

