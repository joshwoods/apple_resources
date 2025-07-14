

- ActivityKit
- Activity
- Activity.ContentStateUpdates
-  Activity.ContentStateUpdates.Iterator Deprecated

Structure

# Activity.ContentStateUpdates.Iterator

An iterator for accessing individual data entries from the series.

iOS 16.1–16.2DeprecatediPadOS 16.1–16.2Deprecated

``` source
struct Iterator
```

Deprecated

Use \`ContentUpdates\` instead

## Topics

### Instance Methods

func next() async -> Activity&lt;Attributes>.ContentStateUpdates.Element?

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

func makeAsyncIterator() -> Activity&lt;Attributes>.ContentStateUpdates.Iterator

Creates the asynchronous iterator that produces results from this asynchronous sequence.

Deprecated

typealias Element

The type of element this asynchronous sequence produces.

Deprecated

