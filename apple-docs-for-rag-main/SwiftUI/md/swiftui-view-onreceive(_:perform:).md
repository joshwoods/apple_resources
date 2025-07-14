

- SwiftUI
- View
-  onReceive(\_:perform:) 

Instance Method

# onReceive(\_:perform:)

Adds an action to perform when this view detects data emitted by the given publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func onReceive(
    _ publisher: P,
    perform action: @escaping (P.Output) -> Void
) -> some View where P : Publisher, P.Failure == Never
```

## Parameters 

`publisher`  

The publisher to subscribe to.

`action`  

The action to perform when an event is emitted by `publisher`. The event emitted by publisher is passed as a parameter to `action`.

## Return Value

A view that triggers `action` when `publisher` emits an event.

## See Also

### Responding to data changes

func onChange(of:initial:_:)

Adds a modifier for this view that fires an action when a specific value changes.

