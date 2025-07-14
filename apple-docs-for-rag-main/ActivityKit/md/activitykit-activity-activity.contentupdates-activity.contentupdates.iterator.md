

- ActivityKit
- Activity
- Activity.ContentUpdates
-  Activity.ContentUpdates.Iterator 

Structure

# Activity.ContentUpdates.Iterator

An iterator for accessing individual data entries from the series.

iOS 16.2+iPadOS 16.2+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() async -> Activity&lt;Attributes>.ContentUpdates.Element?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

