

- ProximityReader
- PaymentCardReader
-  readerIdentifier 

Instance Property

# readerIdentifier

The unique identifier for this card reader.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
var readerIdentifier: String { get async throws }
```

## Discussion

Include this identifier in support requests or tracing incidents to help track down potential problems. If the identifier isn’t readable, getting this value throws a PaymentCardReaderError.

## See Also

### Getting the configuration details

let options: PaymentCardReader.Options

The defined configuration settings when the reader was created.

