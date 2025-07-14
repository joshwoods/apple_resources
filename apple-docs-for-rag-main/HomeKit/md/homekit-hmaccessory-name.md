

- HomeKit
- HMAccessory
-  name 

Instance Property

# name

The name of the accessory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var name: String { get }
```

## Discussion

Use the updateName(_:completionHandler:) method to change the name to a value chosen by the user.

## See Also

### Identifying an Accessory

func updateName(String, completionHandler: ((any Error)?) -> Void)

Changes the name of the accessory.

var uniqueIdentifier: UUID

A unique identifier for the accessory.

var identifier: UUID

A unique identifier for the accessory.

Deprecated

