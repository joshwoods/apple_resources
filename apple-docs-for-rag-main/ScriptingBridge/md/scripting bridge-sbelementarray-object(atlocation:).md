

- Scripting Bridge
- SBElementArray
-  object(atLocation:) 

Instance Method

# object(atLocation:)

Returns the object at the given location in the receiver.

Mac Catalyst 13.0+macOS 10.5+

``` source
func object(atLocation location: Any) -> Any
```

## Return Value

A reference to the SBObject object identified by `loc` or `nil` if the object couldn’t be located.

## Discussion

This method is a generalization of objectAtIndex: for applications where the “index” is not simply an integer. For example, Finder can specify objects using a NSURL object as a location. In OSA this is known as “absolute position,” a generalization of the notion of “index” in Foundation—it could be an integer, but it doesn’t have to be. A single object may even have a number of different “absolute position” values depending on the container.

## See Also

### Getting Objects in the Array

func object(withName: String) -> Any

Returns the object in the array with the given name.

func object(withID: Any) -> Any

Returns the object in the array with the given identifier.

