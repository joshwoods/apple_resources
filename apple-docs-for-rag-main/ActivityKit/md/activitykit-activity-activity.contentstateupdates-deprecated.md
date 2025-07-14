

- ActivityKit
- Activity
-  Activity.ContentStateUpdates Deprecated

Structure

# Activity.ContentStateUpdates

A structure that offers functionality to observe changes to the dynamic content of a Live Activity.

iOS 16.1–16.2DeprecatediPadOS 16.1–16.2Deprecated

``` source
struct ContentStateUpdates
```

Available when `Attributes` conforms to `ActivityAttributes`.

Deprecated

Use \`ContentUpdates\` instead

## Topics

### Creating an iterator

func makeAsyncIterator() -> Activity&lt;Attributes>.ContentStateUpdates.Iterator

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

### Deprecated symbols

static func request(attributes: Attributes, contentState: Activity&lt;Attributes>.ContentState, pushType: PushType?) throws -> Activity&lt;Attributes>

Requests and starts a Live Activity.

Deprecated

var contentState: Activity&lt;Attributes>.ContentState

The dynamic content of a Live Activity.

Deprecated

func update(using: Activity&lt;Attributes>.ContentState, alertConfiguration: AlertConfiguration?) async

Updates the dynamic content of a Live Activity and alerts a person about the Live Activity update.

Deprecated

func end(using: Activity&lt;Attributes>.ContentState?, dismissalPolicy: ActivityUIDismissalPolicy) async

Ends an active Live Activity.

Deprecated

var contentStateUpdates: Activity&lt;Attributes>.ContentStateUpdates

An asynchronous sequence you use to observe changes to the dynamic content of a Live Activity.

Deprecated

