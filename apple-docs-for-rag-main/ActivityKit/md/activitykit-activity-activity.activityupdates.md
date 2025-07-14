

- ActivityKit
- Activity
-  Activity.ActivityUpdates 

Structure

# Activity.ActivityUpdates

A structure that offers functionality to observe changes to a Live Activity.

iOS 16.1+iPadOS 16.1+

``` source
struct ActivityUpdates
```

Available when `Attributes` conforms to `ActivityAttributes`.

## Topics

### Creating an iterator

func makeAsyncIterator() -> Activity&lt;Attributes>.ActivityUpdates.Iterator

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

### Accessing Live Activities

static var activities: [Activity&lt;Attributes>]

An array of your app’s current Live Activities.

static var activityUpdates: Activity&lt;Attributes>.ActivityUpdates

An asynchronous sequence you use to observe changes to ongoing Live Activities and to asynchronously access a Live Activity when you start it.

