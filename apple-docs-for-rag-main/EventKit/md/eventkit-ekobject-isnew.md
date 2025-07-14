

- EventKit
- EKObject
-  isNew 

Instance Property

# isNew

A Boolean value that indicates whether this object has ever been saved.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 6.0+

``` source
var isNew: Bool { get }
```

## Discussion

The value of this property is true if the object hasn’t been saved; otherwise, false.

## See Also

### Saving and Restoring State

var hasChanges: Bool

Returns whether this object or any of the objects it contains has uncommitted changes.

func refresh() -> Bool

Merges changes to this object with the latest saved values.

func reset()

Returns this object to its saved state.

func rollback()

Rolls back the property values of this object to its original state when it was first fetched.

