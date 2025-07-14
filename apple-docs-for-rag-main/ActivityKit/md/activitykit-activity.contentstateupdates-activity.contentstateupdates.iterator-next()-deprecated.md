

- ActivityKit
- Activity
- 
  - Activity
- Activity.ContentStateUpdates
- Activity.ContentStateUpdates.Iterator
-  next() Deprecated

Instance Method

# next()

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

iOS 16.1–16.2DeprecatediPadOS 16.1–16.2Deprecated

``` source
func next() async -> Activity.ContentStateUpdates.Element?
```

Deprecated

Use \`ContentUpdates\` instead

## Return Value

The next element, if it exists, or `nil` to signal the end of the sequence.

