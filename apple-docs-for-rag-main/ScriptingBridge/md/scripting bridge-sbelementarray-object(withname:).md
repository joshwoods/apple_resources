

- Scripting Bridge
- SBElementArray
-  object(withName:) 

Instance Method

# object(withName:)

Returns the object in the array with the given name.

Mac Catalyst 13.0+macOS 10.5+

``` source
func object(withName name: String) -> Any
```

## Parameters 

`name`  

The name of one of the receiver’s objects.

## Return Value

A reference to the designated object or `nil` if the object couldn’t be found.

## Discussion

This method is provided as an alternative to objectAtIndex: for applications where a name is available instead of (or in addition to) an index. A name is generally more stable than an index. For example, it is typically more useful to identify a mailbox in Mail by its name than by its index in the list of mailboxes.

## See Also

### Getting Objects in the Array

func object(withID: Any) -> Any

Returns the object in the array with the given identifier.

func object(atLocation: Any) -> Any

Returns the object at the given location in the receiver.

