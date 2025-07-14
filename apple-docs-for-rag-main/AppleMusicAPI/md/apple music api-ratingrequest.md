

- Apple Music API
-  RatingRequest 

Object

# RatingRequest

A request containing the data for a rating.

Apple Music 1.0+

``` source
object RatingRequest
```

## Properties

`attributes`

RatingRequest.Attributes

 (Required) 

The dictionary that includes the value for the resource’s rating.

`type`

`string`

 (Required) 

The type of the payload.

Value: `ratings`

## Topics

### Related Objects

object RatingRequest.Attributes

The attributes for a rating request object.

## See Also

### Handling the Response

object Ratings

An object that represents a rating for a resource.

object RatingsResponse

The response to a request for a rating.

