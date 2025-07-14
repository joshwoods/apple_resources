

- Apple Music API
-  Activities 

Object

# Activities

A resource object that represents an activity curator.

Apple Music 1.0+

``` source
object Activities
```

## Properties

`id`

`string`

 (Required) 

The identifier for the activity.

`type`

`string`

 (Required) 

This value must always be `activities`.

Value: `activities`

`href`

`string`

 (Required) 

The relative location for the activity resource.

`attributes`

Activities.Attributes

The attributes for the activity.

`relationships`

Activities.Relationships

The relationships for the activity.

## Topics

### Related Objects

object Activities.Attributes

The attributes for an activities resource.

object Activities.Relationships

The relationships for an activity resource.

## See Also

### Handling the Response

object ActivitiesResponse

The response to a request for activities.

