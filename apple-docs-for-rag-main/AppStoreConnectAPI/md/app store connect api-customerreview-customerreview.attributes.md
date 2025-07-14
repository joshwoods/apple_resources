

- App Store Connect API
- CustomerReview
-  CustomerReview.Attributes 

Object

# CustomerReview.Attributes

The attributes of the customer’s review including its content.

App Store Connect API 2.0+

``` source
object CustomerReview.Attributes
```

## Properties

`body`

`string`

The review text that the customer wrote.

`createdDate`

`date-time`

The date and time the customer created the review.

`rating`

`integer`

The rating the customer provided.

Minimum: `1`

Maximum: `5`

`reviewerNickname`

`string`

The customer’s nickname used in the review.

`title`

`string`

The title that the customer wrote for the review.

`territory`

TerritoryCode

The App Store territory.

## Topics

### Types

type TerritoryCode

The App Store territory codes.

## See Also

### Objects

object CustomerReview.Relationships

The relationships you included in the request and those on which you can operate.

