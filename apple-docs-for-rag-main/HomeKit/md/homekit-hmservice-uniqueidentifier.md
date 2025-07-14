

- HomeKit
- HMService
-  uniqueIdentifier 

Instance Property

# uniqueIdentifier

A unique identifier for the service.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var uniqueIdentifier: UUID { get }
```

## See Also

### Identifying the service

var name: String

The user specified name of the service.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the service to the specified string.

