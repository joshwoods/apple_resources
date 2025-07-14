

- Network
- NWBrowser
-  NWBrowser.Result 

Structure

# NWBrowser.Result

A set of discovered services and changes from the last result.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Result
```

## Topics

### Evaluating Browser Results

let endpoint: NWEndpoint

The discovered service endpoint.

let interfaces: [NWInterface]

The list of interfaces on which the service was discovered.

let metadata: NWBrowser.Result.Metadata

The metadata associated with the discovered service, such as the TXT record.

enum Metadata

Values associated with discovered services, such as TXT records.

struct NWTXTRecord

A dictionary representing a TXT record in a DNS packet.

### Comparing Results

enum Change

Ways in which discovered services can change between specific results.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Browsing for Services

init(for: NWBrowser.Descriptor, using: NWParameters)

Initializes a browser with a type of service to discover.

enum Descriptor

A service description used to discover Bonjour services.

func start(queue: DispatchQueue)

Starts browsing for services, and sets the queue on which all browser events will be delivered.

var browseResultsChangedHandler: ((Set&lt;NWBrowser.Result>, Set&lt;NWBrowser.Result.Change>) -> Void)?

A handler that delivers updates about discovered services.

var browseResults: Set&lt;NWBrowser.Result>

The list of discovered services.

