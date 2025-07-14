

- Network
- NWBrowser
-  stateUpdateHandler 

Instance Property

# stateUpdateHandler

A handler that receives browser state updates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency
final var stateUpdateHandler: ((NWBrowser.State) -> Void)? { get set }
```

## See Also

### Managing Browsers

enum State

States indicating whether a browser is able to discover services.

var state: NWBrowser.State

The current state of the browser.

func cancel()

Stops browsing for services.

