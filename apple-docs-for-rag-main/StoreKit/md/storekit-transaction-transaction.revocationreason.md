

- StoreKit
- Transaction
-  Transaction.RevocationReason 

Structure

# Transaction.RevocationReason

Reasons that describe why the App Store may refund a transaction or revoke it from Family Sharing.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct RevocationReason
```

## Topics

### Revocation reasons

static let developerIssue: Transaction.RevocationReason

The value that indicates a customer canceled the transaction due to an actual or perceived issue within your app.

static let other: Transaction.RevocationReason

The value that indicates a customer canceled the transaction for other reasons.

### Getting a localized description

var localizedDescription: String

The localized text that describes the revocation reason.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting revocation status

let revocationDate: Date?

The date that the App Store refunded the transaction or revoked it from Family Sharing.

let revocationReason: Transaction.RevocationReason?

The reason that the App Store refunded the transaction or revoked it from Family Sharing.

