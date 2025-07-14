

- Scripting Bridge
- SBElementArray
-  object(withID:) 

Instance Method

# object(withID:)

Returns the object in the array with the given identifier.

Mac Catalyst 13.0+macOS 10.5+

``` source
func object(withID identifier: Any) -> Any
```

## Parameters 

`identifier`  

The identifier of one of the receiver’s objects.

## Return Value

A reference to the identified object or `nil` if could not be found.

## Discussion

This method is provided as an alternative to objectAtIndex: for applications where an identifier is available instead of (or in addition to) an index. A unique ID is generally more stable than an index. For example, it may be more useful to identify a contact in Address Book by its identifier (which doesn’t change over time) than by its index in the list of contacts (which can change as contacts are added or removed).

## See Also

### Getting Objects in the Array

func object(withName: String) -> Any

Returns the object in the array with the given name.

func object(atLocation: Any) -> Any

Returns the object at the given location in the receiver.

