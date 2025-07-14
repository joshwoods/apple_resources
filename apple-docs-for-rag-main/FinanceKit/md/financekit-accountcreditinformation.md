

- FinanceKit
-  AccountCreditInformation 

Structure

# AccountCreditInformation

A structure that describes the credit information associated with an account.

iOS 17.4+iPadOS 17.4+

``` source
struct AccountCreditInformation
```

## Overview

Credit information includes credit limits, payment dates, and minimum payment dates and amounts for current and upcoming payments.

## Topics

### Operators

static func == (AccountCreditInformation, AccountCreditInformation) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

let creditLimit: CurrencyAmount?

The credit limit of the account.

var hashValue: Int

The hash value.

let minimumNextPaymentAmount: CurrencyAmount?

Minimum amount of the next non-overdue payment.

let nextPaymentDueDate: Date?

Date of the next payment.

let overduePaymentAmount: CurrencyAmount?

The amount by which the account is overdue for the current period.

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

### Transactions

func transactionHistory(forAccountID: UUID, since: FinanceStore.HistoryToken?, isMonitoring: Bool) -> FinanceStore.History&lt;Transaction>

Returns the transactions for the specified account ID, optional starting time, and monitoring indicator for long running transaction queries.

func transactions(query: TransactionQuery) async throws -> [Transaction]

Returns transactions that match the provided transaction query.

struct AccountQuery

A structure that defines an account query.

struct CurrencyAmount

A structure that describes a monetary amount and its currency.

struct Transaction

A structure that represents a transaction relating to a specific financial account.

struct TransactionQuery

A structure that describes the parameters to use for a transaction query.

enum TransactionType

Values that describe kinds of transactions.

enum TransactionStatus

Values that describe the status of a transaction.

