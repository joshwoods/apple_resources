

- FinanceKit
-  Account 

Enumeration

# Account

A structure that describes a financial account.

iOS 17.4+iPadOS 17.4+

``` source
enum Account
```

## Overview

Accounts can include a variety of financial account types such as a bank account, a credit card, or a college fund.

## Topics

### Operators

static func == (Account, Account) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case asset(AssetAccount)

An asset account.

case liability(LiabilityAccount)

A liability account.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var accountDescription: String?

A person’s description of this account.

var assetAccount: AssetAccount?

An asset account.

var currencyCode: String

The ISO 4217 currency code that identifies the currency that denominates the account.

var displayName: String

The name for this account that a person provided.

var id: UUID

The unique account ID for this account.

var institutionName: String

The name of the institution that holds this account.

var liabilityAccount: LiabilityAccount?

A liability account.

var openingDate: Date?

The date the account was opened, if known.

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

### Accounts

func accounts(query: AccountQuery) async throws -> [Account]

Returns a list of accounts a person added to their Wallet that meet the criteria in the provided account query.

func accountHistory(since: FinanceStore.HistoryToken?, isMonitoring: Bool) -> FinanceStore.History&lt;Account>

Returns a list of accounts a person added since a time specified by the provided financial history token.

struct AssetAccount

A structure that describes the characteristics of an asset account.

struct LiabilityAccount

A structure that describes the characteristics of a liability account.

