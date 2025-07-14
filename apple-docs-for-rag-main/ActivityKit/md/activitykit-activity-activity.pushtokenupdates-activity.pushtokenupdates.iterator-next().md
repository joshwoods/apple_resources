

- ActivityKit
- Activity
- Activity.PushTokenUpdates
- Activity.PushTokenUpdates.Iterator
-  next() 

Instance Method

# next()

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

iOS 16.1+iPadOS 16.1+

``` source
func next() async -> Activity.PushTokenUpdates.Element?
```

## Return Value

The next element, if it exists, or `nil` to signal the end of the sequence.

