

- ActivityKit
- ActivityAuthorizationInfo
-  ActivityAuthorizationInfo.ActivityEnablementUpdates 

Structure

# ActivityAuthorizationInfo.ActivityEnablementUpdates

A structure that offers functionality to observe whether your app can start a Live Activity.

iOS 16.1+iPadOS 16.1+

``` source
struct ActivityEnablementUpdates
```

## Topics

### Creating an iterator

func makeAsyncIterator() -> ActivityAuthorizationInfo.ActivityEnablementUpdates.Iterator

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

### Observing Live Activity permission changes

var areActivitiesEnabled: Bool

A Boolean value that indicates whether your app can start a Live Activity.

let activityEnablementUpdates: ActivityAuthorizationInfo.ActivityEnablementUpdates

An asynchronous sequence you use to observe whether your app can start a Live Activity.

init()

Creates an object you use to observe user authorizations for starting Live Activities and updating them with ActivityKit push notifications.

