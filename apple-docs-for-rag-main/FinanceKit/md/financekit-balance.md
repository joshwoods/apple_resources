

- FinanceKit
-  Balance 

Structure

# Balance

A structure that describes an account balance.

iOS 17.4+iPadOS 17.4+

``` source
struct Balance
```

## Topics

### Operators

static func == (Balance, Balance) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

let amount: CurrencyAmount

The amount of the balance.

let asOfDate: Date

The date and time the system calculated the balance.

let creditDebitIndicator: CreditDebitIndicator

A value that indicates whether the balance is a credit or a debit balance.

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
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

enum CreditDebitIndicator

Values that the framework uses to describe transactions as credits or debits.

enum CurrentBalance

Values that describe the state of an account’s credit balance.

