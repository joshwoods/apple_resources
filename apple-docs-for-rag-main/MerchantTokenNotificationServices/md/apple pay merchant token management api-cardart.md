

- Apple Pay Merchant Token Management API
-  CardArt 

Object

# CardArt

Data for displaying art to represent a card.

App Store Connect API 1.0.10+

``` source
object CardArt
```

## Properties

`name`

`string`

 (Required) 

A name representing the bank and the card used for the transaction.

Minimum length: `1`

Maximum length: `64`

`type`

`string`

 (Required) 

The card type.

Minimum length: `1`

Maximum length: `64`

`url`

`string`

 (Required) 

The URL for downloading the card art, as provided by the issuing bank.

Minimum length: `1`

Maximum length: `128`

## See Also

### Merchant token event retrieval

Get Details of a Merchant Token Event

Get the details of a merchant token event after receiving a notification.

object MerchantTokenEventResponse

A response body that contains information about a life-cycle event for a merchant token.

object MerchantTokenMetadata

The card information related to a merchant token, including its card art and metadata.

object CardMetadata

Data about the card, including its expiration date and suffix.

