

- ActivityKit
- ActivityAuthorizationInfo
- ActivityAuthorizationInfo.FrequentPushEnablementUpdates
-  ActivityAuthorizationInfo.FrequentPushEnablementUpdates.Iterator 

Structure

# ActivityAuthorizationInfo.FrequentPushEnablementUpdates.Iterator

An iterator for accessing individual data entries from the series.

iOS 16.2+iPadOS 16.2+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() async -> Bool?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

## See Also

### Creating an iterator

func makeAsyncIterator() -> ActivityAuthorizationInfo.FrequentPushEnablementUpdates.Iterator

Creates the asynchronous iterator that produces results from this asynchronous sequence.

typealias Element

The type of element this asynchronous sequence produces.

