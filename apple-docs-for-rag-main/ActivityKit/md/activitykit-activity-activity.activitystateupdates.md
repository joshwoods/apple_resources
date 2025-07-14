

- ActivityKit
- Activity
-  Activity.ActivityStateUpdates 

Structure

# Activity.ActivityStateUpdates

A structure that offers functionality to observe state changes of a Live Activity.

iOS 16.1+iPadOS 16.1+

``` source
struct ActivityStateUpdates
```

Available when `Attributes` conforms to `ActivityAttributes`.

## Topics

### Creating an iterator

func makeAsyncIterator() -> Activity&lt;Attributes>.ActivityStateUpdates.Iterator

Creates the asynchronous iterator that produces results from this asynchronous sequence.

struct Iterator

An iterator for accessing individual data entries from the series.

typealias Element

The type of element this asynchronous sequence produces.

### Type Aliases

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Observing the Live Activity life cycle

var activityState: ActivityState

The current state of a Live Activity in its life cycle.

enum ActivityState

The enum that describes the state of a Live Activity in its life cycle.

var activityStateUpdates: Activity&lt;Attributes>.ActivityStateUpdates

An asynchronous sequence you use to observe activity state changes.

