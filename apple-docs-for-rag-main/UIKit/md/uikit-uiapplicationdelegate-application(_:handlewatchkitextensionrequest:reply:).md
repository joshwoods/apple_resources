

- UIKit
- UIApplicationDelegate
-  application(\_:handleWatchKitExtensionRequest:reply:) 

Instance Method

# application(\_:handleWatchKitExtensionRequest:reply:)

Asks the delegate to respond to a request from a paired watchOS app.

iOS 8.2+iPadOS 8.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    handleWatchKitExtensionRequest userInfo: [AnyHashable : Any]?,
    reply: @escaping ([AnyHashable : Any]?) -> Void
)
```

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    handleWatchKitExtensionRequest userInfo: [AnyHashable : Any]?
) async -> [AnyHashable : Any]?
```

## Parameters 

`application`  

Your singleton app object.

`userInfo`  

A dictionary provided by the watchOS app with the request information. Use the data in this dictionary to process the request from the watchOS app.

`reply`  

A block to execute with the results of the request. This block has no return value and takes the following parameter:

replyInfo  
A dictionary containing data to return to the watchOS app. The contents of the dictionary must be serializable to a property list file. The contents of this dictionary are at your discretion and you may specify `nil`.

## Discussion

If your iOS app and watchOS app coordinate efforts to perform certain tasks, implement this method and use it to respond to requests from the watchOS app. After finishing the request, execute the provided `reply` block (if any) to return the results.

Because this method is likely to be called while your app is in the background, call the beginBackgroundTask(withName:expirationHandler:) method at the start of your implementation and the endBackgroundTask(_:) method after you have processed the reply and executed the `reply` block. Starting a background task ensures that your app is not suspended before it has a chance to send its reply.

