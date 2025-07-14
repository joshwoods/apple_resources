

- ActivityKit
- Activity
-  Activity.ContentUpdates 

Structure

# Activity.ContentUpdates

A structure that offers functionality to observe changes to the dynamic content of a Live Activity.

iOS 16.2+iPadOS 16.2+

``` source
struct ContentUpdates
```

Available when `Attributes` conforms to `ActivityAttributes`.

## Topics

### Structures

struct Iterator

An iterator for accessing individual data entries from the series.

### Instance Methods

func makeAsyncIterator() -> Activity&lt;Attributes>.ContentUpdates.Iterator

Creates the asynchronous iterator that produces results from this asynchronous sequence.

### Type Aliases

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

The type of element this asynchronous sequence produces.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Observing Live Activity content changes

var contentUpdates: Activity&lt;Attributes>.ContentUpdates

An asynchronous sequence you use to observe changes to the dynamic content of a Live Activity.

