

- FinanceKit
-  TransactionStatus 

Enumeration

# TransactionStatus

Values that describe the status of a transaction.

iOS 17.4+iPadOS 17.4+

``` source
enum TransactionStatus
```

## Topics

### Enumeration Cases

case authorized

The transaction is in an authorized state.

case booked

The transaction is in a booked state.

case memo

A memo that provides information about the transaction.

case pending

The transaction is in a pending state.

case rejected

The transaction is in a rejected state.

### Initializers

init?(rawValue: Int16)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: Int16

The corresponding value of the raw type.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static var allCases: [TransactionStatus]

A collection of all values of this type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- CaseIterable
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Transactions

func transactionHistory(forAccountID: UUID, since: FinanceStore.HistoryToken?, isMonitoring: Bool) -> FinanceStore.History&lt;Transaction>

Returns the transactions for the specified account ID, optional starting time, and monitoring indicator for long running transaction queries.

func transactions(query: TransactionQuery) async throws -> [Transaction]

Returns transactions that match the provided transaction query.

struct AccountQuery

A structure that defines an account query.

struct AccountCreditInformation

A structure that describes the credit information associated with an account.

struct CurrencyAmount

A structure that describes a monetary amount and its currency.

struct Transaction

A structure that represents a transaction relating to a specific financial account.

struct TransactionQuery

A structure that describes the parameters to use for a transaction query.

enum TransactionType

Values that describe kinds of transactions.

