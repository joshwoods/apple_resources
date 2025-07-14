

- Service Management
- SMAppService
-  unregister(completionHandler:) 

Instance Method

# unregister(completionHandler:)

Unregisters the service so the system no longer launches it and calls a completion handler you provide with the resulting error value.

Mac Catalyst 16.0+macOS 13.0+

``` source
func unregister(completionHandler handler: @escaping ((any Error)?) -> Void)
```

``` source
func unregister() async throws
```

## Parameters 

`handler`  

A completion handler to call with the result of the unregistration operation. Upon an unsuccessful return, the handler contains a new NSError object describing the error. Upon successful return, this argument is `NULL`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Registering services

func register() throws

Registers the service so it can begin launching subject to user approval.

func unregister() throws

Unregisters the service so the system no longer launches it.

