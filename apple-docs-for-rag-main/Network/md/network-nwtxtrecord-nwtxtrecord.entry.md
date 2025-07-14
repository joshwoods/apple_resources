

- Network
- NWTXTRecord
-  NWTXTRecord.Entry 

Enumeration

# NWTXTRecord.Entry

A type of entry in a TXT record dictionary.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Entry
```

## Topics

### Entry Types

case none

The key is not mapped to any value.

case empty

The key is mapped to an empty value.

case string(String)

The key is mapped to a string.

### Enumeration Cases

case data(Data)

### Initializers

init(Data?)

### Instance Properties

var data: Data?

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Creating TXT Records

init([String : String])

Initializes a TXT record with a dictionary of strings.

func removeEntry(key: String) -> Bool

Removes an entry from a TXT record dictionary.

func setEntry(NWTXTRecord.Entry, for: String) -> Bool

Sets an entry in a TXT record dictionary.

