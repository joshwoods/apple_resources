

- App Intents
-  IntentCurrencyAmount 

Structure

# IntentCurrencyAmount

An amount of money to transfer during a financial transaction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentCurrencyAmount
```

## Topics

### Creating a currency type

init(amount: Decimal, currencyCode: String)

Creates a IntentCurrencyAmount from a monetary amount and a currency code.

### Getting the currency details

let amount: Decimal

The monetary amount.

let currencyCode: String

The ISO 4217 currency code that applies to the monetary amount.

### Operators

static func == (IntentCurrencyAmount, IntentCurrencyAmount) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias Specification

typealias UnwrappedType

typealias ValueType

### Type Properties

static var defaultResolverSpecification: EmptyResolverSpecification&lt;IntentCurrencyAmount>

### Default Implementations

Equatable Implementations

InstanceDisplayRepresentable Implementations

TypeDisplayRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- CustomLocalizedStringResourceConvertible
- DisplayRepresentable
- Equatable
- Hashable
- InstanceDisplayRepresentable
- Sendable
- TypeDisplayRepresentable

## See Also

### Monetary types

struct IntentPaymentMethod

Information about a form of payment supported by your app.

