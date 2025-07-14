

- DeviceCheck
- DCDevice
-  generateToken(completionHandler:) 

Instance Method

# generateToken(completionHandler:)

Generates a token that identifies the current device.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+tvOS 11.0+visionOS 1.0+watchOS 9.0+

``` source
func generateToken(completionHandler completion: @escaping (Data?, (any Error)?) -> Void)
```

``` source
func generateToken() async throws -> Data
```

## Parameters 

`completion`  

A completion block that includes the following parameters:

- `token`: An ephemeral token that identifies the current device.

- `error`: The error that occurred, if any.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func generateToken() async throws -> Data
```

For example:

```
let token = try await generateToken()
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Your server uses the generated token in its requests to get or set the persistent bits for the current device. You should treat the token you receive in the completion block as single-use. Although the token remains valid long enough for your server to retry a specific request if necessary, you should not use a token multiple times. Instead, use this method to generate a new token.

Note

The app you use to generate the token must be associated with your developer account; otherwise, the generation request fails.

