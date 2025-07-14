

- FinanceKit
-  Transaction 

Structure

# Transaction

A structure that represents a transaction relating to a specific financial account.

iOS 17.4+iPadOS 17.4+

``` source
struct Transaction
```

## Overview

This can include transactions such as a deposit to or a withdrawn from bank account, a credit card transaction.

## Topics

### Operators

static func == (Transaction, Transaction) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

let accountID: UUID

The account ID the transaction belongs to.

let creditDebitIndicator: CreditDebitIndicator

An indicator that describes if the transaction is a credit or a debit.

let foreignCurrencyAmount: CurrencyAmount?

The total amount of the transaction, if it was carried out in a foreign currency.

let foreignCurrencyExchangeRate: Decimal?

The currency exchange rate, if the transaction was carried out in a foreign currency.

let id: UUID

A unique internal ID.

let merchantCategoryCode: MerchantCategoryCode?

The ISO 18245 category code for the transaction.

let merchantName: String?

The name of the merchant, if present.

let originalTransactionDescription: String

The unmodified description of the transaction.

let postedDate: Date?

The date and time that the transaction was posted to the account.

let status: TransactionStatus

The status of the transaction, if available.

let transactionAmount: CurrencyAmount

The total amount of the transaction.

let transactionDate: Date

The time the transaction took place, if available.

let transactionDescription: String

A description of the transaction.

let transactionType: TransactionType

The type of the transaction.

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

struct TransactionQuery

A structure that describes the parameters to use for a transaction query.

enum TransactionType

Values that describe kinds of transactions.

enum TransactionStatus

Values that describe the status of a transaction.

