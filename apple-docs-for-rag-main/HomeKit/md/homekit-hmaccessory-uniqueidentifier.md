

- HomeKit
- HMAccessory
-  uniqueIdentifier 

Instance Property

# uniqueIdentifier

A unique identifier for the accessory.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var uniqueIdentifier: UUID { get }
```

## See Also

### Identifying an Accessory

var name: String

The name of the accessory.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Changes the name of the accessory.

var identifier: UUID

A unique identifier for the accessory.

Deprecated

