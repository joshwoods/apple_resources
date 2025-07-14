

- Address Book
- ABRecord
-  setValue(\_:forProperty:) 

Instance Method

# setValue(\_:forProperty:)

Sets the value of a given property for a record.

macOS

``` source
func setValue(
    _ value: Any!,
    forProperty property: String!
) -> Bool
```

## Parameters 

`value`  

The value to set for `property`.

`property`  

The property whose value will be set.

## Return Value

`true` if the value was set successfully; otherwise, `false`.

## Discussion

The type of the value must match the property’s type (see Property Types for a list of possible property types). If `property` is `nil` or if `value` is not of the correct type, this method raises an exception. If `property` is a multivalue list property, this method checks to see if the values in the multivalue list are the same type. If the multivalue list contains mixed types, the value will not be set successfully.

For a list of the available properties, see Accessing Address Book Records in Address Book Programming Guide for Mac.

## See Also

### Retrieving and Setting Values

func removeValue(forProperty: String!) -> Bool

Removes the value for a given property.

func setValue(Any!, forProperty: String!, error: ()) throws

Sets the value of a given property for a record, returning error information.

func value(forProperty: String!) -> Any!

Returns the value of a given property for a record.

