

- Core Data
- NSManagedObject
-  willChangeValue(forKey:withSetMutation:using:) 

Instance Method

# willChangeValue(forKey:withSetMutation:using:)

Provides an opportunity to respond when a change is about to be made to a specified to-many relationship.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func willChangeValue(
    forKey inKey: String,
    withSetMutation inMutationKind: NSKeyValueSetMutationKind,
    using inObjects: Set
)
```

## Parameters 

`inKey`  

The name of a property that is a to-many relationship

`inMutationKind`  

The type of change that will be made.

`inObjects`  

The objects that were involved in the change (see NSKeyValueSetMutationKind).

## Discussion

For more details, see Key-Value Observing Programming Guide.

You must not override this method.

## See Also

### Supporting Key-Value Observing

func didAccessValue(forKey: String?)

Provides support for key-value observing access notification.

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

