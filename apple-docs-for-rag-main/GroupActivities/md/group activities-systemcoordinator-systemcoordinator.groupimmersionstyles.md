

- Group Activities
- SystemCoordinator
-  SystemCoordinator.GroupImmersionStyles 

Structure

# SystemCoordinator.GroupImmersionStyles

An asynchronous sequence that contains one or more incoming immersion styles for you to process.

GroupActivitiesSwiftUIvisionOS 1.0+

``` source
struct GroupImmersionStyles
```

## Overview

When a participant in an activity changes the immersion style of their immersive space, the system adds the style to this sequence. Configure an asynchronous task to monitor this sequence and process results when they arrive.

The following example shows you how to configure this task and use it to iterate over the available items. The `systemCoordinator` variable contains the session’s SystemCoordinator object.

```
Task.detached {
    for await immersionStyle in systemCoordinator.groupImmersionStyle {
        if let immersionStyle {
            // Open an immersive space with the same style.
        }
        else {
            // Dismiss the immersive space.
        }
    }
}
```

## Topics

### Classes

class Iterator

### Instance Methods

func makeAsyncIterator() -> SystemCoordinator.GroupImmersionStyles.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

### Type Aliases

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

The type of element produced by this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Getting the current immersion level

var groupImmersionStyle: SystemCoordinator.GroupImmersionStyles

The presentation style to apply to an immersive space for the current activity.

