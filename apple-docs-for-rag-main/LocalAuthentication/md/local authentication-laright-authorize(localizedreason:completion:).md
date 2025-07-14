

- Local Authentication
- LARight
-  authorize(localizedReason:completion:) 

Instance Method

# authorize(localizedReason:completion:)

Performs an authorization on the right.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func authorize(
    localizedReason: String,
    completion handler: @escaping ((any Error)?) -> Void
)
```

``` source
func authorize(localizedReason: String) async throws
```

## Parameters 

`localizedReason`  

A reason for the authorization that the system displays to the user.

`handler`  

A completion handler called at the end of the authorization process.

`error`  
If `nil`, the authorization is successful. Otherwise, the error contains information about the failure reason.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func authorize(localizedReason: String) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Authorizing a right

init()

Creates a right using the default authorization requirements.

init(requirement: LAAuthenticationRequirement)

Creates a right with the authentication requirements you supply.

var tag: Int

An integer you use to identify a right.

func authorize(localizedReason: String, in: LAPresentationContext, completion: ((any Error)?) -> Void)

Performs an authorization on the right with a window context you supply.

