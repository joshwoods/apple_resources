

- ManagedApp
- ManagedAppError
-  ManagedAppError.serverError 

Case

# ManagedAppError.serverError

An error that indicates a failure requesting a secret from the asset server.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

``` source
case serverError
```

## Discussion

This error can also indicate a problem communicating with a subsequent server, such as ACME or SCEP.

