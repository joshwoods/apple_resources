

- Apple Music API
-  Ratings 

Object

# Ratings

An object that represents a rating for a resource.

Apple Music 1.0+

``` source
object Ratings
```

## Properties

`id`

`string`

 (Required) 

The identifier for the rating.

`type`

`string`

 (Required) 

This value is always `ratings`.

Value: `ratings`

`href`

`string`

 (Required) 

The relative location for the playlist resource.

`attributes`

Ratings.Attributes

The attributes for the rating.

`relationships`

Ratings.Relationships

The relationships from ratings to other resources.

## Topics

### Related Objects

object Ratings.Attributes

The attributes for a rating resource.

object Ratings.Relationships

The relationships for a rating resource.

## See Also

### Handling the Response

object RatingsResponse

The response to a request for a rating.

object RatingRequest

A request containing the data for a rating.

