

- FinanceKit
-  AccountBalance 

Structure

# AccountBalance

A structure that describes the financial balance of an account at a specific point in time.

iOS 17.4+iPadOS 17.4+

``` source
struct AccountBalance
```

## Topics

### Operators

static func == (AccountBalance, AccountBalance) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

let accountID: UUID

The account ID the balance belongs to.

var available: Balance?

The available balance, if present.

var booked: Balance?

The booked balance, if present.

var currencyCode: String

The balance currency.

let currentBalance: CurrentBalance

The balance at a particular moment in time.

let id: UUID

A unique account balance ID.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Identifiable
- Sendable

## See Also

### Balances

func accountBalances(query: AccountBalanceQuery) async throws -> [AccountBalance]

Returns a list of balances that meet the criteria in the provided account query.

func accountBalanceHistory(forAccountID: UUID, since: FinanceStore.HistoryToken?, isMonitoring: Bool) -> FinanceStore.History&lt;AccountBalance>

Returns the account balance history since a time specified by the provided financial history token.

struct AccountBalanceQuery

A structure that defines an account balance query.

struct Balance

A structure that describes an account balance.

enum CreditDebitIndicator

Values that the framework uses to describe transactions as credits or debits.

enum CurrentBalance

Values that describe the state of an account’s credit balance.

