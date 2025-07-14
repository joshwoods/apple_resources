

- ActivityKit
- ActivityAuthorizationInfo
- ActivityAuthorizationInfo.ActivityEnablementUpdates
-  ActivityAuthorizationInfo.ActivityEnablementUpdates.Iterator 

Structure

# ActivityAuthorizationInfo.ActivityEnablementUpdates.Iterator

An iterator for accessing individual data entries from the series.

iOS 16.1+iPadOS 16.1+

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

func makeAsyncIterator() -> ActivityAuthorizationInfo.ActivityEnablementUpdates.Iterator

Creates the asynchronous iterator that produces results from this asynchronous sequence.

typealias Element

The type of element this asynchronous sequence produces.

