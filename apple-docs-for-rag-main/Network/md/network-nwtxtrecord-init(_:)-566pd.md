

- Network
- NWTXTRecord
-  init(\_:) 

Initializer

# init(\_:)

Initializes a TXT record with a dictionary of strings.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(_ dictionary: [String : String] = [:])
```

## See Also

### Creating TXT Records

func removeEntry(key: String) -> Bool

Removes an entry from a TXT record dictionary.

func setEntry(NWTXTRecord.Entry, for: String) -> Bool

Sets an entry in a TXT record dictionary.

enum Entry

A type of entry in a TXT record dictionary.

