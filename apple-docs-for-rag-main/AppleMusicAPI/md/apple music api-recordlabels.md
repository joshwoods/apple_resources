

- Apple Music API
-  RecordLabels 

Object

# RecordLabels

A resource object that represents a record label.

Apple Music 1.0+

``` source
object RecordLabels
```

## Properties

`id`

`string`

 (Required) 

The identifier for the record label.

`type`

`string`

 (Required) 

This value must always be `record-labels`.

Value: `record-labels`

`href`

`string`

 (Required) 

A relative location for the record label resource.

`attributes`

RecordLabels.Attributes

The attributes of the record label.

`views`

RecordLabels.Views

The relationship views for the record label.

## Topics

### Related Objects

object RecordLabels.Attributes

The attributes for a record label resource.

object RecordLabels.Views

The relationship views for a record label resource.

## See Also

### Handling the Response

object RecordLabelsResponse

The response to a request for record labels.

