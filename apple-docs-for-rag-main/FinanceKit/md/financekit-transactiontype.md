

- FinanceKit
-  TransactionType 

Enumeration

# TransactionType

Values that describe kinds of transactions.

iOS 17.4+iPadOS 17.4+

``` source
enum TransactionType
```

## Topics

### Enumeration Cases

case adjustment

A credit or debit adjustment transaction.

case atm

An ATM transaction.

case billPayment

A bill payment, usually carried out through an eBill or eCheck system.

case check

A check payment.

case deposit

A deposit of money by a payer into a payee’s bank account.

case directDebit

A payment to a third party on agreed dates, typically in order to pay bills.

case directDeposit

A deposit of money by a payer directly into a payee’s bank account.

case dividend

A distribution of a company’s earnings to its shareholders.

case fee

A fee or charge levied by the account provider.

case interest

A credit or debit due to interest earned or incurred.

case loan

A loan drawdown or repayment.

case pointOfSale

A Point of Sales transaction.

case refund

A refund.

case standingOrder

A regular payment of a fixed amount that’s paid on a specified date.

case transfer

A transfer between accounts.

case unknown

The transaction’s category doesn’t map to a known value.

case withdrawal

An automatic or recurring withdrawal of funds by another party.

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

static var allCases: [TransactionType]

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

enum TransactionStatus

Values that describe the status of a transaction.

