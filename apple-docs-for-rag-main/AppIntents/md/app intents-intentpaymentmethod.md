

- App Intents
-  IntentPaymentMethod 

Structure

# IntentPaymentMethod

Information about a form of payment supported by your app.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentPaymentMethod
```

## Overview

An `IntentPaymentMethod` type describes a way someone pays for goods and services. This type contains information you can display in your interface to convey the payment type to people. Specifically, it stores the name of the payment service and an icon for any related brand information. Typical payment methods include credit cards and bank accounts.

## Topics

### Creating a payment method

init(type: IntentPaymentMethod.PaymentType, name: LocalizedStringResource?, identificationHint: String?, icon: DisplayRepresentation.Image?)

### Getting the payment details

var paymentType: IntentPaymentMethod.PaymentType

The kind of payment method, such as a credit card or bank account

var name: String?

The user-visible name of the payment method

var identificationHint: String?

A hint making it easier for the user to identify the payment method among others of similar name or type, such as the last several digits of a credit card number

var icon: DisplayRepresentation.Image?

The icon or image representing this payment method

enum PaymentType

Constants that describe the available payment options, such as credit cards or bank accounts.

### Type Aliases

typealias Specification

typealias UnwrappedType

typealias ValueType

### Type Properties

static var defaultResolverSpecification: EmptyResolverSpecification&lt;IntentPaymentMethod>

### Default Implementations

InstanceDisplayRepresentable Implementations

TypeDisplayRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- CustomLocalizedStringResourceConvertible
- DisplayRepresentable
- InstanceDisplayRepresentable
- Sendable
- TypeDisplayRepresentable

## See Also

### Monetary types

struct IntentCurrencyAmount

An amount of money to transfer during a financial transaction.

