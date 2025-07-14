

- EventKit
- EKObject
-  reset() 

Instance Method

# reset()

Returns this object to its saved state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 6.0+

``` source
func reset()
```

## Discussion

This method updates all the properties of this object with the corresponding values in the event store. Any local changes that were not saved before invoking this method are lost. This method does nothing if the object was never saved.

## See Also

### Saving and Restoring State

var hasChanges: Bool

Returns whether this object or any of the objects it contains has uncommitted changes.

var isNew: Bool

A Boolean value that indicates whether this object has ever been saved.

func refresh() -> Bool

Merges changes to this object with the latest saved values.

func rollback()

Rolls back the property values of this object to its original state when it was first fetched.

