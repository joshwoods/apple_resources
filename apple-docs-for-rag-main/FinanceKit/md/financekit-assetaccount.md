

- FinanceKit
-  AssetAccount 

Structure

# AssetAccount

A structure that describes the characteristics of an asset account.

iOS 17.4+iPadOS 17.4+

``` source
struct AssetAccount
```

## Overview

An asset account includes accounts such as a bank account or a savings account.

## Topics

### Operators

static func == (AssetAccount, AssetAccount) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

let accountDescription: String?

The description of the account.

let currencyCode: String

ISO 4217 currency code that identifies the currency in which the account is held.

let displayName: String

The name for the account given by a person.

let id: UUID

A unique account identifier.

let institutionName: String

The name of the institution that holds the account.

let openingDate: Date?

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

struct LiabilityAccount

A structure that describes the characteristics of a liability account.

enum Account

A structure that describes a financial account.

