

- Network
- NWTXTRecord
-  dictionary 

Instance Property

# dictionary

The TXT record as a dictionary of strings.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var dictionary: [String : String] { get }
```

## See Also

### Examining TXT Records

func getEntry(for: String) -> NWTXTRecord.Entry?

Accesses an entry in a TXT record dictionary.

subscript(String) -> String?

Get and set values in a TXT record dictionary, by keys.

