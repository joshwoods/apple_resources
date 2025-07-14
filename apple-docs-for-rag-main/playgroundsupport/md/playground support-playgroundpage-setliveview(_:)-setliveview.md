

- Playground Support
- PlaygroundPage
-  setLiveView(\_:) 

Generic Instance Method

# setLiveView(\_:)

Displays a view that shows the result of running the code that’s on the current page.

macOS 11.0+Xcode 12.0+Swift Playgrounds 4.0+

**macOS**

``` source
final func setLiveView(_ newLiveView: IncomingView) where IncomingView : PlaygroundLiveViewable
```

**Swift Playgrounds**

``` source
func setLiveView(_ newLiveView: IncomingView) where IncomingView : PlaygroundLiveViewable
```

## Parameters 

`newLiveView`  

The view to display as the current page’s live view.

## Discussion

The live view appears in the assistant editor for the current playground page. There can be only one live view open at any time.

When you call `setLiveView(_:)`, the system sets needsIndefiniteExecution to `true`.

## See Also

### Configuring Live Views

static let current: PlaygroundPage

The current playground page.

func setLiveView&lt;IncomingView>(IncomingView)

Displays a SwiftUI view that shows the result of running the code that’s on the current page.

var liveView: (any PlaygroundLiveViewable)?

A live view that shows the result of running the code that’s on the current page.

