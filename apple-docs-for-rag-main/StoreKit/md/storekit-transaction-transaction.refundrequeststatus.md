

- StoreKit
- Transaction
-  Transaction.RefundRequestStatus 

Enumeration

# Transaction.RefundRequestStatus

The status codes for refund requests.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum RefundRequestStatus
```

## Overview

The following methods throw the refund request status: beginRefundRequest(in:), beginRefundRequest(for:in:), beginRefundRequest(in:), and beginRefundRequest(for:in:).

The refund request status reflects the status of the request, not the status of the refund itself.

## Topics

### Getting Refund Request Status

case userCancelled

The user canceled submission of their refund request.

case success

The App Store has received the refund request.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
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

enum RefundRequestError

The error codes for refund requests.

