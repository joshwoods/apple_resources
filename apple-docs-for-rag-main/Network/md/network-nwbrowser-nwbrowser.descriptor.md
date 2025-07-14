

- Network
- NWBrowser
-  NWBrowser.Descriptor 

Enumeration

# NWBrowser.Descriptor

A service description used to discover Bonjour services.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Descriptor
```

## Topics

### Descriptor Types

case bonjour(type: String, domain: String?)

A service descriptor used to discover a Bonjour service.

case bonjourWithTXTRecord(type: String, domain: String?)

A service descriptor used to discover a Bonjour service with associated TXT records.

### Enumeration Cases

case applicationService(name: String)

Returns a browser descriptor for application services.

## Relationships

### Conforms To

- Sendable

## See Also

### Browsing for Services

init(for: NWBrowser.Descriptor, using: NWParameters)

Initializes a browser with a type of service to discover.

func start(queue: DispatchQueue)

Starts browsing for services, and sets the queue on which all browser events will be delivered.

var browseResultsChangedHandler: ((Set&lt;NWBrowser.Result>, Set&lt;NWBrowser.Result.Change>) -> Void)?

A handler that delivers updates about discovered services.

struct Result

A set of discovered services and changes from the last result.

var browseResults: Set&lt;NWBrowser.Result>

The list of discovered services.

