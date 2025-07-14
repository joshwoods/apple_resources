

- HomeKit
- HMHome
-  isPrimary 

Instance Property

# isPrimary

A Boolean value that indicates whether this is the primary home for its home manager.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var isPrimary: Bool { get }
```

## See Also

### Identifying a home

var name: String

The name the user gives to the home.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the home.

var uniqueIdentifier: UUID

A unique identifier for the home.

