

- Group Activities
- GroupSessionMessenger
-  GroupSessionMessenger.Messages 

Structure

# GroupSessionMessenger.Messages

An asynchronous sequence of messages sent to the session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct Messages where Message : Decodable, Message : Encodable
```

## Overview

When you use a GroupSessionMessenger to communicate across devices, the `Messages` structure provides the sequence of messages the other devices send. Iterate over the contents of this structure asynchronously to retrieve each message and update your app.

Don’t create this structure directly. Instead, use the messages(of:) or messages(of:) method to retrieve the messages for a given session.

## Topics

### Creating an iterator

func makeAsyncIterator() -> GroupSessionMessenger.Messages&lt;Message>.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

struct Iterator

typealias Element

The type of element produced by this asynchronous sequence.

### Finding elements

func contains(where: (Self.Element) async throws -> Bool) async rethrows -> Bool

Returns a Boolean value that indicates whether the asynchronous sequence contains an element that satisfies the given predicate.

func allSatisfy((Self.Element) async throws -> Bool) async rethrows -> Bool

Returns a Boolean value that indicates whether all elements produced by the asynchronous sequence satisfy the given predicate.

func first(where: (Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the first element of the sequence that satisfies the given predicate.

func min(by: (Self.Element, Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the minimum element in the asynchronous sequence, using the given predicate as the comparison between elements.

func max(by: (Self.Element, Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the maximum element in the asynchronous sequence, using the given predicate as the comparison between elements.

### Selecting elements

func prefix(Int) -> AsyncPrefixSequence&lt;Self>

Returns an asynchronous sequence, up to the specified maximum length, containing the initial elements of the base asynchronous sequence.

func prefix(while: (Self.Element) async -> Bool) rethrows -> AsyncPrefixWhileSequence&lt;Self>

Returns an asynchronous sequence, containing the initial, consecutive elements of the base sequence that satisfy the given predicate.

### Excluding elements

func dropFirst(Int) -> AsyncDropFirstSequence&lt;Self>

Omits a specified number of elements from the base asynchronous sequence, then passes through all remaining elements.

func drop(while: (Self.Element) async -> Bool) -> AsyncDropWhileSequence&lt;Self>

Omits elements from the base asynchronous sequence until a given closure returns false, after which it passes through all remaining elements.

func filter((Self.Element) async -> Bool) -> AsyncFilterSequence&lt;Self>

Creates an asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given predicate.

### Transforming a sequence

func reduce&lt;Result>(Result, (Result, Self.Element) async throws -> Result) async rethrows -> Result

Returns the result of combining the elements of the asynchronous sequence using the given closure.

func reduce&lt;Result>(into: Result, (inout Result, Self.Element) async throws -> Void) async rethrows -> Result

Returns the result of combining the elements of the asynchronous sequence using the given closure, given a mutable initial value.

### Type Aliases

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Receiving data from other participants

func messages(of: Data.Type) -> GroupSessionMessenger.Messages&lt;Data>

Returns the asynchronous sequence of messages that contain a generic data object.

func messages&lt;Message>(of: Message.Type) -> GroupSessionMessenger.Messages&lt;Message>

Returns the asynchronous sequence of messages that match the app-specific type.

struct MessageContext

A structure that contains additional information about an incoming message, such as which device sent it.

