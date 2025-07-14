

- AVFoundation
- AVAssetResourceLoaderDelegate
-  resourceLoader(\_:didCancel:) 

Instance Method

# resourceLoader(\_:didCancel:)

Informs the delegate that a prior authentication challenge has been cancelled.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func resourceLoader(
    _ resourceLoader: AVAssetResourceLoader,
    didCancel authenticationChallenge: URLAuthenticationChallenge
)
```

## Parameters 

`resourceLoader`  

The resource loader.

`authenticationChallenge`  

The authentication challenge that has been cancelled.

## See Also

### Processing Authentication Challenges

func resourceLoader(AVAssetResourceLoader, shouldWaitForResponseTo: URLAuthenticationChallenge) -> Bool

Tells the delegate that assistance is required of the application to respond to an authentication challenge.

