

- StoreKit
-  PaymentMethodBinding 

Structure

# PaymentMethodBinding

A binding that makes payment methods available in apps for an Apple ID.

iOS 16.4+iPadOS 16.4+visionOS 1.0+

``` source
struct PaymentMethodBinding
```

## Overview

This functionality is available only to eligible apps with server entitlements. The initializer init(id:) throws an error if your app doesn’t have the appropriate entitlement to use this API, or if the user isn’t eligible.

Important

The init(id:) and bind() methods may display a system prompt that asks users to authenticate with their Apple ID. Call these methods only after an explicit user action, like tapping or clicking a button.

Initialize this structure using the in-app binding identifier that your server receives from the Apple server when your server initiates payment method binding. Call the bind() method to prompt users to confirm adding the payment method and making it their primary payment method.

## Topics

### Determining eligiblity

init(id: String) async throws

Creates the payment method binding for eligible apps and users.

### Creating and identifying bindings

let id: String

The in-app binding identifier.

### Binding payment methods

func bind() async throws

Asks the user to confirm whether to add the payment method to their Apple payment methods.

### Reading errors

enum PaymentMethodBindingError

Error information for payment method binding.

## Relationships

### Conforms To

- Equatable
- Hashable
- Identifiable
- Sendable

