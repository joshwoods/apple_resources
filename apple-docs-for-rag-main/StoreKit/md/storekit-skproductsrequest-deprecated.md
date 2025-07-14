

- StoreKit
-  SKProductsRequest Deprecated

Class

# SKProductsRequest

An object that can retrieve localized information from the App Store about a specified list of products.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
class SKProductsRequest
```

Deprecated

Use Product.products(for:)

## Mentioned in 

Testing a product request

Implementing introductory offers in your app

Fetching product information from the App Store

Implementing promotional offers in your app

## Overview

Your app uses an SKProductsRequest object to present localized prices and other information to the user without having to maintain that list of product information itself.

To use an SKProductsRequest object, you initialize it with a list of product identifier strings, attach a delegate, and then call the request’s start() method. When the request completes, your delegate receives an SKProductsResponse object.

Note

Be sure to keep a strong reference to the request object; otherwise, the system might deallocate the request before it can complete.

## Topics

### Initializing a Products Request

init(productIdentifiers: Set&lt;String>)

Initializes the request with the set of product identifiers.

### Setting the Delegate

var delegate: (any SKProductsRequestDelegate)?

The delegate that receives the response of the app’s products request.

protocol SKProductsRequestDelegate

A set of methods the delegate implements so it receives the product information your app requests.

## Relationships

### Inherits From

- SKRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Product information

Loading in-app product identifiers

Load the unique identifiers for your in-app products to retrieve product information from the App Store.

Fetching product information from the App Store

Retrieve up-to-date information about the products for sale in your app to display to your customers.

class SKProductsResponse

An App Store response to a request for information about a list of products.

Deprecated

class SKProduct

Information about a registered product in App Store Connect.

Deprecated

