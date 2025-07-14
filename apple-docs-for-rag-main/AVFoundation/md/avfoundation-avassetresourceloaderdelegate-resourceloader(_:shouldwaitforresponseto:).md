

- AVFoundation
- AVAssetResourceLoaderDelegate
-  resourceLoader(\_:shouldWaitForResponseTo:) 

Instance Method

# resourceLoader(\_:shouldWaitForResponseTo:)

Tells the delegate that assistance is required of the application to respond to an authentication challenge.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func resourceLoader(
    _ resourceLoader: AVAssetResourceLoader,
    shouldWaitForResponseTo authenticationChallenge: URLAuthenticationChallenge
) -> Bool
```

## Parameters 

`resourceLoader`  

The resource loader.

`authenticationChallenge`  

The authentication challenge.

## Return Value

true if the resource loader should wait for a response to the authentication challenge; otherwise false.

## Discussion

Delegates receive this message when assistance is required of the application to respond to an authentication challenge.

Return true if you expect a response either subsequently or immediately to the authenticationChallenger object’s sender.

If you intend to respond to the authentication challenge after your handling of `resourceLoader:shouldWaitForResponseToAuthenticationChallenge:` returns, you must retain the authenticationChallenge until after your response has been made.

## See Also

### Processing Authentication Challenges

func resourceLoader(AVAssetResourceLoader, didCancel: URLAuthenticationChallenge)

Informs the delegate that a prior authentication challenge has been cancelled.

