

- Core Data
- NSManagedObject
-  willAccessValue(forKey:) 

Instance Method

# willAccessValue(forKey:)

Provides support for key-value observing access notification.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func willAccessValue(forKey key: String?)
```

## Parameters 

`key`  

The name of one of the receiver’s properties.

## Discussion

See didAccessValue(forKey:) for more details. You can invoke this method with the `key` value of `nil` to ensure that a fault has been fired, as illustrated by the following example.

```
[aManagedObject willAccessValueForKey:nil];
```

## See Also

### Supporting Key-Value Observing

func didAccessValue(forKey: String?)

Provides support for key-value observing access notification.

func observationInfo() -> UnsafeMutableRawPointer?

Returns the observation info of the managed object.

func setObservationInfo(UnsafeMutableRawPointer?)

Sets the observation info of the managed object.

func didChangeValue(forKey: String)

Provides an opportunity to respond when a value of a given property has changed.

func didChangeValue(forKey: String, withSetMutation: NSKeyValueSetMutationKind, using: Set&lt;AnyHashable>)

Provides an opportunity to respond when a change was made to a specified to-many relationship.

func willChangeValue(forKey: String)

Provides an opportunity to respond when a value of a given property is about to change.

func willChangeValue(forKey: String, withSetMutation: NSKeyValueSetMutationKind, using: Set&lt;AnyHashable>)

Provides an opportunity to respond when a change is about to be made to a specified to-many relationship.

