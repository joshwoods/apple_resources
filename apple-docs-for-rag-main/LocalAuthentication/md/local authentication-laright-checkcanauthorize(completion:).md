

- Local Authentication
- LARight
-  checkCanAuthorize(completion:) 

Instance Method

# checkCanAuthorize(completion:)

Checks whether the right has permission to perform authorization.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func checkCanAuthorize(completion handler: @escaping ((any Error)?) -> Void)
```

``` source
func checkCanAuthorize() async throws
```

## Parameters 

`handler`  

A completion handler called when the authorization check finishes.

`error`  
If `nil`, the right can be authorized.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func checkCanAuthorize() async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Monitoring authorization status

var state: LARight.State

The current authorization state for a right.

enum State

The possible states for a right during authorization.

