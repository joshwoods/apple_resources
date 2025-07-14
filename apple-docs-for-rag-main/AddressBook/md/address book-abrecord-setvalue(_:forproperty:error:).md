

- Address Book
- ABRecord
-  setValue(\_:forProperty:error:) 

Instance Method

# setValue(\_:forProperty:error:)

Sets the value of a given property for a record, returning error information.

macOS 10.7+

``` source
func setValue(
    _ value: Any!,
    forProperty property: String!,
    error: ()
) throws
```

## Parameters 

`value`  

The value to set for `property`.

`property`  

The property whose value will be set.

`error`  

A pointer to an error object that is set to an NSError instance if an error occurs.

## Discussion

The type of the value must match the property’s type (see Property Types for a list of possible property types). If `property` is `nil` or if `value` is not of the correct type, this method raises an exception. If `property` is a multivalue list property, this method checks to see if the values in the multivalue list are the same type. If the multivalue list contains mixed types, the value will not be set successfully.

For a list of the available properties, see Accessing Address Book Records in Address Book Programming Guide for Mac.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Retrieving and Setting Values

func removeValue(forProperty: String!) -> Bool

Removes the value for a given property.

func setValue(Any!, forProperty: String!) -> Bool

Sets the value of a given property for a record.

func value(forProperty: String!) -> Any!

Returns the value of a given property for a record.

