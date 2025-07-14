

- Core Data
- NSManagedObject
-  objectIDs(forRelationshipNamed:) 

Instance Method

# objectIDs(forRelationshipNamed:)

Returns the object IDs for all of the managed objects that are in the named relationship.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func objectIDs(forRelationshipNamed key: String) -> [NSManagedObjectID]
```

## See Also

### Supporting Key-Value Coding

func value(forKey: String) -> Any?

Returns the value for the property specified by `key`.

func setValue(Any?, forKey: String)

Sets the specified property of the managed object to the specified value.

func primitiveValue(forKey: String) -> Any?

Returns the value for the specified property from the managed object’s private internal storage .

func setPrimitiveValue(Any?, forKey: String)

Sets the value of a given property in the managed object’s private internal storage.

