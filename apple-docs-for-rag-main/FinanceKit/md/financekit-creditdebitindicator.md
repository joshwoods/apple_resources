

- FinanceKit
-  CreditDebitIndicator 

Enumeration

# CreditDebitIndicator

Values that the framework uses to describe transactions as credits or debits.

iOS 17.4+iPadOS 17.4+

``` source
enum CreditDebitIndicator
```

## Topics

### Enumeration Cases

case credit

A value that indicates an amount which increases an asset or decreases a liability.

case debit

A value that indicates an amount which increases a liability or decreases an asset.

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

static var allCases: [CreditDebitIndicator]

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

### Balances

func accountBalances(query: AccountBalanceQuery) async throws -> [AccountBalance]

Returns a list of balances that meet the criteria in the provided account query.

func accountBalanceHistory(forAccountID: UUID, since: FinanceStore.HistoryToken?, isMonitoring: Bool) -> FinanceStore.History&lt;AccountBalance>

Returns the account balance history since a time specified by the provided financial history token.

struct AccountBalance

A structure that describes the financial balance of an account at a specific point in time.

struct AccountBalanceQuery

A structure that defines an account balance query.

struct Balance

A structure that describes an account balance.

enum CurrentBalance

Values that describe the state of an account’s credit balance.

