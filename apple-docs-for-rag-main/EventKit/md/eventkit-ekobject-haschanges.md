

- EventKit
- EKObject
-  hasChanges 

Instance Property

# hasChanges

Returns whether this object or any of the objects it contains has uncommitted changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 6.0+

``` source
var hasChanges: Bool { get }
```

## Return Value

Returns true if there are uncommitted changes; otherwise, false.

## See Also

### Saving and Restoring State

var isNew: Bool

A Boolean value that indicates whether this object has ever been saved.

func refresh() -> Bool

Merges changes to this object with the latest saved values.

func reset()

Returns this object to its saved state.

func rollback()

Rolls back the property values of this object to its original state when it was first fetched.

