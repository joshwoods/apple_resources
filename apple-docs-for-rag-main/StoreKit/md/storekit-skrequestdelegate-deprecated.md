

- StoreKit
-  SKRequestDelegate Deprecated

Protocol

# SKRequestDelegate

Common methods that are implemented by delegates for any subclass of the `SKRequest` abstract class.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
protocol SKRequestDelegate : NSObjectProtocol
```

Deprecated

No longer supported

## Topics

### Completing Requests

func requestDidFinish(SKRequest)

Tells the delegate that the request has completed.

### Handling Errors

func request(SKRequest, didFailWithError: any Error)

Tells the delegate that the request failed to execute.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- SKProductsRequestDelegate

## See Also

### Accessing the Delegate

var delegate: (any SKRequestDelegate)?

The delegate of the request object.

Deprecated

