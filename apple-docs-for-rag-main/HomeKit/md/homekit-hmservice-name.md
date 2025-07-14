

- HomeKit
- HMService
-  name 

Instance Property

# name

The user specified name of the service.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var name: String { get }
```

## Discussion

Rename services by calling the updateName(_:completionHandler:) method with a value given by the user.

## See Also

### Identifying the service

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the service to the specified string.

var uniqueIdentifier: UUID

A unique identifier for the service.

