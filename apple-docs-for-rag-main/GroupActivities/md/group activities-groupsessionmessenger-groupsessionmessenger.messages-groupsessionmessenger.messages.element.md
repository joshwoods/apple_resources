

- Group Activities
- GroupSessionMessenger
- GroupSessionMessenger.Messages
-  GroupSessionMessenger.Messages.Element 

Type Alias

# GroupSessionMessenger.Messages.Element

The type of element produced by this asynchronous sequence.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
typealias Element = (Message, GroupSessionMessenger.MessageContext)
```

## See Also

### Creating an iterator

func makeAsyncIterator() -> GroupSessionMessenger.Messages&lt;Message>.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

struct Iterator

