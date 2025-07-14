

- StoreKit
- SKRequestDelegate
-  request(\_:didFailWithError:) Deprecated

Instance Method

# request(\_:didFailWithError:)

Tells the delegate that the request failed to execute.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
optional func request(
    _ request: SKRequest,
    didFailWithError error: any Error
)
```

Deprecated

No longer supported

## Parameters 

`request`  

The request that failed.

`error`  

The error that caused the request to fail.

## Mentioned in 

Handling errors

## Discussion

When the request fails, your application should release the request. The requestDidFinish(_:) method is not called after this method is called.

