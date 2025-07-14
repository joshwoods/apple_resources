

- Core Data
- NSManagedObject
-  primitiveValue(forKey:) 

Instance Method

# primitiveValue(forKey:)

Returns the value for the specified property from the managed object’s private internal storage .

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func primitiveValue(forKey key: String) -> Any?
```

## Parameters 

`key`  

The name of one of the receiver’s properties.

## Return Value

The value of the property specified by `key`. Returns `nil` if no value has been set.

## Discussion

This method does not invoke the access notification methods (willAccessValue(forKey:) and didAccessValue(forKey:)). This method is used primarily by subclasses that implement custom accessor methods that need direct access to the receiver’s private storage.

### Special Considerations

Subclasses should not override this method.

The following points also apply:

- Primitive accessor methods are only supported on *modeled* properties. If you invoke a primitive accessor on an unmodeled property, it will instead operate upon a random modeled property. (The debug libraries and frameworks (available from Apple Developer Website) have assertions to test for passing unmodeled keys to these methods.)

- You are strongly encouraged to use the dynamically-generated accessors rather than using this method directly (for example, `primitiveName:` instead of `primitiveValueForKey:@"name"`). The dynamic accessors are much more efficient, and allow for compile-time checking.

## See Also

### Related Documentation

func setObservationInfo(UnsafeMutableRawPointer?)

Sets the observation info of the managed object.

### Supporting Key-Value Coding

func value(forKey: String) -> Any?

Returns the value for the property specified by `key`.

func setValue(Any?, forKey: String)

Sets the specified property of the managed object to the specified value.

func setPrimitiveValue(Any?, forKey: String)

Sets the value of a given property in the managed object’s private internal storage.

func objectIDs(forRelationshipNamed: String) -> [NSManagedObjectID]

Returns the object IDs for all of the managed objects that are in the named relationship.

