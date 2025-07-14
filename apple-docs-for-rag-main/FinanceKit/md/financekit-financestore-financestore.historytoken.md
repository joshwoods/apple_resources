

- FinanceKit
- FinanceStore
-  FinanceStore.HistoryToken 

Structure

# FinanceStore.HistoryToken

A structure that describes the starting point to use for financial data queries.

iOS 17.4+iPadOS 17.4+

``` source
struct HistoryToken
```

## Topics

### Initializers

init(from: any Decoder) throws

Initializes a new history token using data from the provided decoder.

### Instance Methods

func encode(to: any Encoder) throws

Persists a the history token data using the provided encoder.

## Relationships

### Conforms To

- Decodable
- Encodable
- Sendable

## See Also

### Orders

struct FullyQualifiedOrderIdentifier

A structure that specifies the characteristics of an order.

func saveOrder(signedArchive: Data) async throws -> FinanceStore.SaveOrderResult

Adds an order to the store or updates an existing order.

