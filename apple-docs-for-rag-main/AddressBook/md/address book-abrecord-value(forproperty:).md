

- Address Book
- ABRecord
-  value(forProperty:) 

Instance Method

# value(forProperty:)

Returns the value of a given property for a record.

macOS

``` source
func value(forProperty property: String!) -> Any!
```

## Parameters 

`property`  

The property whose value will be returned.

## Return Value

The value of the given property.

## Discussion

The type of the value depends on the property type (see Property Types for a list of possible property types). Note that the returned value is always of an immutable type (for example, an `NSString` type, not an `NSMutableString` type, is returned).

If `property` is `nil`, this method raises an exception. If `property` is invalid, this method returns `nil`.

For a list of the available properties, see Accessing Address Book Records in Address Book Programming Guide for Mac.

## See Also

### Retrieving and Setting Values

func removeValue(forProperty: String!) -> Bool

Removes the value for a given property.

func setValue(Any!, forProperty: String!) -> Bool

Sets the value of a given property for a record.

func setValue(Any!, forProperty: String!, error: ()) throws

Sets the value of a given property for a record, returning error information.

