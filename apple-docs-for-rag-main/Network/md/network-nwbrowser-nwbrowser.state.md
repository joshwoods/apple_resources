

- Network
- NWBrowser
-  NWBrowser.State 

Enumeration

# NWBrowser.State

States indicating whether a browser is able to discover services.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum State
```

## Topics

### States

case setup

The browser has been initialized but not started.

case ready

The browser is registered for discovering services.

case failed(NWError)

The browser has encountered a fatal error.

case cancelled

The browser has been canceled.

### Enumeration Cases

case waiting(NWError)

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Managing Browsers

var stateUpdateHandler: ((NWBrowser.State) -> Void)?

A handler that receives browser state updates.

var state: NWBrowser.State

The current state of the browser.

func cancel()

Stops browsing for services.

