

- Group Activities
- GroupSessionJournal
- GroupSessionJournal.Attachments
- GroupSessionJournal.Attachments.Iterator
-  next() 

Instance Method

# next()

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
mutating func next() async -> GroupSessionJournal.Attachments.Element?
```

## Return Value

The next element, if it exists, or `nil` to signal the end of the sequence.

