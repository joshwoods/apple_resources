

- Core Data
- NSManagedObject
-  observationInfo() 

Instance Method

# observationInfo()

Returns the observation info of the managed object.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+

``` source
func observationInfo() -> UnsafeMutableRawPointer?
```

## Return Value

The observation info of the receiver.

## Discussion

For more about key-value observation, see Key-Value Observing Programming Guide.

Important

You must not override this method.

## See Also

### Supporting Key-Value Observing

func didAccessValue(forKey: String?)

Provides support for key-value observing access notification.

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

