

- Core Data
- NSManagedObject
-  didAccessValue(forKey:) 

Instance Method

# didAccessValue(forKey:)

Provides support for key-value observing access notification.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func didAccessValue(forKey key: String?)
```

## Parameters 

`key`  

The name of one of the receiver’s properties.

## Discussion

Together with willAccessValue(forKey:), this method is used to fire faults, to maintain inverse relationships, and so on. Each read access must be wrapped in this method pair (in the same way that each write access must be wrapped in the `willChangeValueForKey:`/`didChangeValueForKey:` method pair). In the default implementation of `NSManagedObject` these methods are invoked for you automatically. If, say, you create a custom subclass that uses explicit instance variables, you must invoke them yourself, as in the following example.

```
- (NSString *)firstName
{
    [self willAccessValueForKey:@"firstName"];
    NSString *rtn = firstName;
    [self didAccessValueForKey:@"firstName"];
    return rtn;
}
```

## See Also

### Supporting Key-Value Observing

func observationInfo() -> UnsafeMutableRawPointer?

Returns the observation info of the managed object.

func setObservationInfo(UnsafeMutableRawPointer?)

Sets the observation info of the managed object.

func willAccessValue(forKey: String?)

Provides support for key-value observing access notification.

func didChangeValue(forKey: String)

Provides an opportunity to respond when a value of a given property has changed.

func didChangeValue(forKey: String, withSetMutation: NSKeyValueSetMutationKind, using: Set&lt;AnyHashable>)

Provides an opportunity to respond when a change was made to a specified to-many relationship.

func willChangeValue(forKey: String)

Provides an opportunity to respond when a value of a given property is about to change.

func willChangeValue(forKey: String, withSetMutation: NSKeyValueSetMutationKind, using: Set&lt;AnyHashable>)

Provides an opportunity to respond when a change is about to be made to a specified to-many relationship.

