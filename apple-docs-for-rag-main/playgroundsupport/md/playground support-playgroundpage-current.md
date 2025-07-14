

- Playground Support
- PlaygroundPage
-  current 

Type Property

# current

The current playground page.

macOS 11.0+Xcode 10.2+Swift Playgrounds 2.0+

``` source
static let current: PlaygroundPage
```

## Discussion

Use `current` to find the playground page instance.

## See Also

### Configuring Live Views

func setLiveView&lt;IncomingView>(IncomingView)

Displays a SwiftUI view that shows the result of running the code that’s on the current page.

func setLiveView&lt;IncomingView>(IncomingView)

Displays a view that shows the result of running the code that’s on the current page.

var liveView: (any PlaygroundLiveViewable)?

A live view that shows the result of running the code that’s on the current page.

