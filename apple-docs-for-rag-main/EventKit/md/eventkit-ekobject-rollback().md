

- EventKit
- EKObject
-  rollback() 

Instance Method

# rollback()

Rolls back the property values of this object to its original state when it was first fetched.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 6.0+

``` source
func rollback()
```

## Discussion

Any local changes to this object are lost when invoking this method. This method does not re-fetch property values from the event store. This method does nothing if the object was never changed.

## See Also

### Saving and Restoring State

var hasChanges: Bool

Returns whether this object or any of the objects it contains has uncommitted changes.

var isNew: Bool

A Boolean value that indicates whether this object has ever been saved.

func refresh() -> Bool

Merges changes to this object with the latest saved values.

func reset()

Returns this object to its saved state.

