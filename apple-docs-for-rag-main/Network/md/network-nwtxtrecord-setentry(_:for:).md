

- Network
- NWTXTRecord
-  setEntry(\_:for:) 

Instance Method

# setEntry(\_:for:)

Sets an entry in a TXT record dictionary.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@discardableResult
mutating func setEntry(
    _ entry: NWTXTRecord.Entry,
    for key: String
) -> Bool
```

## See Also

### Creating TXT Records

init([String : String])

Initializes a TXT record with a dictionary of strings.

func removeEntry(key: String) -> Bool

Removes an entry from a TXT record dictionary.

enum Entry

A type of entry in a TXT record dictionary.

