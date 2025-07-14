

- Address Book
- ABRecord
-  removeValue(forProperty:) 

Instance Method

# removeValue(forProperty:)

Removes the value for a given property.

macOS

``` source
func removeValue(forProperty property: String!) -> Bool
```

## Parameters 

`property`  

The property whose value will be removed.

## Return Value

true if the value is removed successfully; otherwise, false.

## Discussion

When you next call value(forProperty:) on that property, it returns `nil`.

If property is `nil`, this method raises an exception.

For a list of the available properties, see Accessing Address Book Records in Address Book Programming Guide for Mac.

## See Also

### Retrieving and Setting Values

func setValue(Any!, forProperty: String!) -> Bool

Sets the value of a given property for a record.

func setValue(Any!, forProperty: String!, error: ()) throws

Sets the value of a given property for a record, returning error information.

func value(forProperty: String!) -> Any!

Returns the value of a given property for a record.

