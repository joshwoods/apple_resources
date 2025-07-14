

- ProximityReader
- MobileDocumentReader
-  configuration 

Instance Property

# configuration

The configuration of the mobile document reader.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
final var configuration: MobileDocumentReader.Configuration { get async throws }
```

## Discussion

Use the information contained in the configuration to construct as reader token on your server.

Throws

A MobileDocumentReaderError if an error occurs.

## See Also

### Retrieving the reader configuration

struct Configuration

A type that represents the configuration of the mobile document reader.

