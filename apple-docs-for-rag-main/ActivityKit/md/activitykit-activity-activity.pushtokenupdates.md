

- ActivityKit
- Activity
-  Activity.PushTokenUpdates 

Structure

# Activity.PushTokenUpdates

A structure that offers functionality to observe changes to the push token of a Live Activity.

iOS 16.1+iPadOS 16.1+

``` source
struct PushTokenUpdates
```

Available when `Attributes` conforms to `ActivityAttributes`.

## Topics

### Creating an iterator

func makeAsyncIterator() -> Activity&lt;Attributes>.PushTokenUpdates.Iterator

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

### Using ActivityKit push notifications

var pushToken: Data?

The token you use to send ActivityKit push notifications to a Live Activity.

var pushTokenUpdates: Activity&lt;Attributes>.PushTokenUpdates

An asynchronous sequence you use to observe changes to the push token of a Live Activity.

static var pushToStartToken: Data?

The token you use to start a Live Activity with an ActivityKit push notification.

static var pushToStartTokenUpdates: Activity&lt;Attributes>.PushTokenUpdates

An asynchronous sequence you use to observe changes to the token for starting a Live Activity with an ActivityKit push notification.

