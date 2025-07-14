

- Network
-  NWTXTRecord 

Structure

# NWTXTRecord

A dictionary representing a TXT record in a DNS packet.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct NWTXTRecord
```

## Topics

### Creating TXT Records

init([String : String])

Initializes a TXT record with a dictionary of strings.

func removeEntry(key: String) -> Bool

Removes an entry from a TXT record dictionary.

func setEntry(NWTXTRecord.Entry, for: String) -> Bool

Sets an entry in a TXT record dictionary.

enum Entry

A type of entry in a TXT record dictionary.

### Examining TXT Records

func getEntry(for: String) -> NWTXTRecord.Entry?

Accesses an entry in a TXT record dictionary.

subscript(String) -> String?

Get and set values in a TXT record dictionary, by keys.

var dictionary: [String : String]

The TXT record as a dictionary of strings.

### Initializers

init(Data)

### Instance Properties

var data: Data

## Relationships

### Conforms To

- Collection
- Copyable
- CustomDebugStringConvertible
- Equatable
- Sendable
- Sequence

## See Also

### Evaluating Browser Results

let endpoint: NWEndpoint

The discovered service endpoint.

let interfaces: [NWInterface]

The list of interfaces on which the service was discovered.

let metadata: NWBrowser.Result.Metadata

The metadata associated with the discovered service, such as the TXT record.

enum Metadata

Values associated with discovered services, such as TXT records.

