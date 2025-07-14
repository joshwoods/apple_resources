

- UIKit
- UIApplicationDelegate
-  application(\_:handlerFor:) 

Instance Method

# application(\_:handlerFor:)

Asks the delegate for an intent handler capable of handling the specified intent.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    handlerFor intent: INIntent
) -> Any?
```

## Parameters 

`application`  

The shared app object.

`intent`  

The intent object that represents the request coming from the system.

## Return Value

An instance of a type capable of handling the specified intent; otherwise, `nil` if your app doesn’t handle the intent. Return an instance of a type that conforms to the handling intents protocol for the same type as the provided intent.

## Discussion

Important

The system only invokes this method in apps that support multiple scenes. For more information, see Specifying the scenes your app supports.

Siri invokes this method on the main queue when it wants to process one of your app’s supported intents. To indicate the intents that your app supports, populate the INIntentsSupported array in your app target’s `Info.plist` file.

In your delegate’s implementation of this method, check the `intent` parameter’s type and return a custom object that adopts the corresponding handling protocol. For example, if `intent` is an instance of doc://com.apple.documentation/documentation/sirikit/inplaymediaintent, return an object that adopts doc://com.apple.documentation/documentation/sirikit/inplaymediaintenthandling. Only use the provided intent to determine the handler to return; don’t use it to initialize the handler and don’t store a reference to it. SiriKit updates the intent throughout the request to incorporate information the requester provides. For more information, see Dispatching intents to handlers.

For information about handling intents, see Resolving and Handling Intents.

