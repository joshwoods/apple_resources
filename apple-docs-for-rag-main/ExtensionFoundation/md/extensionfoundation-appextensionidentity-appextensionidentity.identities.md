

- ExtensionFoundation
- AppExtensionIdentity
-  AppExtensionIdentity.Identities 

Structure

# AppExtensionIdentity.Identities

An asynchronous sequence that returns the enabled extensions that match provided constraints.

macOS 13.0+

``` source
struct Identities
```

## Topics

### Iterating the Sequence

func next() async -> [AppExtensionIdentity]?

Asynchronously advances to the next element and returns it.

struct AsyncIterator

The type of the asynchronous iterator created by this asynchronous sequence.

typealias Element

The type of element produced by this asynchronous sequence.

func makeAsyncIterator() -> AppExtensionIdentity.Identities.AsyncIterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Identifying the Process

var bundleIdentifier: String

The bundle identifier for the extension.

var extensionPointIdentifier: String

A unique identifier for the extension point this extension targets.

var localizedName: String

A localized, human-readable name for the extension.

