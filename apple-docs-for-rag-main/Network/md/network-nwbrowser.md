

- Network
-  NWBrowser 

Class

# NWBrowser

An object you use to browse for available network services.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final class NWBrowser
```

## Topics

### Essentials

NSBonjourServices

Bonjour service types browsed by the app.

NSLocalNetworkUsageDescription

A message that tells the user why the app is requesting access to the local network.

### Browsing for Services

init(for: NWBrowser.Descriptor, using: NWParameters)

Initializes a browser with a type of service to discover.

enum Descriptor

A service description used to discover Bonjour services.

func start(queue: DispatchQueue)

Starts browsing for services, and sets the queue on which all browser events will be delivered.

var browseResultsChangedHandler: ((Set&lt;NWBrowser.Result>, Set&lt;NWBrowser.Result.Change>) -> Void)?

A handler that delivers updates about discovered services.

struct Result

A set of discovered services and changes from the last result.

var browseResults: Set&lt;NWBrowser.Result>

The list of discovered services.

### Managing Browsers

var stateUpdateHandler: ((NWBrowser.State) -> Void)?

A handler that receives browser state updates.

enum State

States indicating whether a browser is able to discover services.

var state: NWBrowser.State

The current state of the browser.

func cancel()

Stops browsing for services.

### Inspecting Browsers

let descriptor: NWBrowser.Descriptor

The service descriptor with which the browser was initialized.

let parameters: NWParameters

The parameters with which the browser was initialized.

var queue: DispatchQueue?

The queue on which browser events are delivered.

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Sendable

## See Also

### Connections and Listeners

class NWConnection

A bidirectional data connection between a local endpoint and a remote endpoint.

class NWListener

An object you use to listen for incoming network connections.

class NWConnectionGroup

An object you use to communicate with a group of endpoints, such as an IP multicast group on a local network.

class NWEthernetChannel

An object you use to send and receive custom Ethernet frames.

