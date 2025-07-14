

- StoreKit
- Transaction
-  Transaction.RefundRequestError 

Enumeration

# Transaction.RefundRequestError

The error codes for refund requests.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum RefundRequestError
```

## Overview

The following methods throw refund request errors: beginRefundRequest(in:), beginRefundRequest(for:in:), beginRefundRequest(in:), and beginRefundRequest(for:in:).

## Topics

### Error Enumeration

case duplicateRequest

The App Store has already received a refund request for this in-app purchase.

case failed

The refund request submission failed.

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- LocalizedError
- Sendable

## See Also

### Requesting refunds

Testing refund requests

Test your app’s implementation of refund requests, and your app’s and server’s handling of approved and declined refunds.

func beginRefundRequest(in: UIWindowScene) async throws -> Transaction.RefundRequestStatus

Presents the refund request sheet for the transaction in a window scene.

func beginRefundRequest(in: NSViewController) async throws -> Transaction.RefundRequestStatus

Presents the refund request sheet for the transaction in a view controller.

static func beginRefundRequest(for: UInt64, in: UIWindowScene) async throws -> Transaction.RefundRequestStatus

Presents the refund request sheet for the specified transaction in a window scene.

static func beginRefundRequest(for: UInt64, in: NSViewController) async throws -> Transaction.RefundRequestStatus

Presents the refund request sheet for the specified transaction in a view controller.

enum RefundRequestStatus

The status codes for refund requests.

