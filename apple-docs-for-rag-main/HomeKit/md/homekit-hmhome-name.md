

- HomeKit
- HMHome
-  name 

Instance Property

# name

The name the user gives to the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var name: String { get }
```

## Discussion

The name should be configured by the user when a new home is created.

## See Also

### Identifying a home

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the home.

var uniqueIdentifier: UUID

A unique identifier for the home.

var isPrimary: Bool

A Boolean value that indicates whether this is the primary home for its home manager.

