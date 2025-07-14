

- HomeKit
- HMHome
-  uniqueIdentifier 

Instance Property

# uniqueIdentifier

A unique identifier for the home.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var uniqueIdentifier: UUID { get }
```

## See Also

### Identifying a home

var name: String

The name the user gives to the home.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the home.

var isPrimary: Bool

A Boolean value that indicates whether this is the primary home for its home manager.

