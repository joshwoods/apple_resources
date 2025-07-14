

- StoreKit Test
-  SKTestError 

Structure

# SKTestError

Information about an error that the testing environment returns.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct SKTestError
```

## Topics

### Error Domain

static var errorDomain: String

The domain of the error.

### Error Codes

static var fileNotFound: SKTestError.Code

The initializer can’t find the file.

static var invalidAction: SKTestError.Code

The action is invalid.

static var invalidProductIdentifier: SKTestError.Code

The product identifier is invalid.

static var invalidProductType: SKTestError.Code

The product type is invalid.

static var invalidURL: SKTestError.Code

The URL is invalid.

static var noSubscriptionFound: SKTestError.Code

The test environment didn’t find a subscription.

static var noTransactionFound: SKTestError.Code

The test environment didn’t find a transaction.

static var serviceUnavailable: SKTestError.Code

The service isn’t available.

enum Code

Error codes in the testing environment.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### StoreKit transaction testing errors

let SKTestErrorDomain: String

A constant that represents the domain for error codes in the testing environment.

