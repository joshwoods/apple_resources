

- Network Extension
- NEProvider
-  displayMessage(\_:completionHandler:) Deprecated

Instance Method

# displayMessage(\_:completionHandler:)

Call this method from your NEProvider subclass if you want to display a message to the person using the app.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedvisionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, visionOS**

``` source
func displayMessage(
    _ message: String,
    completionHandler: @escaping (Bool) -> Void
)
```

**Mac Catalyst, visionOS**

``` source
func displayMessage(_ message: String) async -> Bool
```

## Parameters 

`message`  

The message you want to display to the person using the app.

`completionHandler`  

A block that the system calls after you call this method. The details of the call can vary, as follows:

- If the system can’t display the message, or if you call the `displayMessage:completionHandler:` method in an NEFilterDataProvider instance, then the system calls the `completionHandler` block immediately after you call the method, and sets the block’s `success` parameter value to false.

- If the system successfully displays the message to the user, then the system calls the `completionHandler` block when the user dismisses the message, and sets the `success` parameter value to true.

