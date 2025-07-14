

- ActivityKit
- ActivityAuthorizationInfo
-  ActivityAuthorizationInfo.FrequentPushEnablementUpdates 

Structure

# ActivityAuthorizationInfo.FrequentPushEnablementUpdates

A structure that can observe whether you can update Live Activities with frequent ActivityKit push notifications.

iOS 16.2+iPadOS 16.2+

``` source
struct FrequentPushEnablementUpdates
```

## Topics

### Creating an iterator

func makeAsyncIterator() -> ActivityAuthorizationInfo.FrequentPushEnablementUpdates.Iterator

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

### Observing availability of frequent ActivityKit push notifications

var frequentPushesEnabled: Bool

A Boolean value that indicates whether a person permitted you to update Live Activities with frequent ActivityKit push notifications.

let frequentPushEnablementUpdates: ActivityAuthorizationInfo.FrequentPushEnablementUpdates

An asynchronous sequence you use to observe whether a person permitted you to update Live Activities with frequent ActivityKit push notifications.

