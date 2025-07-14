

- StoreKit
- SKRequestDelegate
-  requestDidFinish(\_:) Deprecated

Instance Method

# requestDidFinish(\_:)

Tells the delegate that the request has completed.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
optional func requestDidFinish(_ request: SKRequest)
```

Deprecated

No longer supported

## Parameters 

`request`  

The request that completed.

## Discussion

This method is called after all processing of the request has been completed. Typically, subclasses of SKRequest require the delegate to implement additional methods to receive the response. When this method is called, your delegate receives no further communication from the request and can release it.

## See Also

### Related Documentation

In-App Purchase Programming Guide

