

- Matter
-  MTRXPCServerProtocol_MTRDeviceController 

Protocol

# MTRXPCServerProtocol_MTRDeviceController

iOS 18.3+iPadOS 18.3+Mac Catalyst 18.3+macOS 15.3+tvOS 18.3+visionOS 2.3+watchOS 11.3+

``` source
protocol MTRXPCServerProtocol_MTRDeviceController : NSObjectProtocol
```

## Topics

### Instance Methods

func deviceController(UUID, deleteNodeID: NSNumber)

func deviceController(UUID, getNodesWithStoredDataWithReply: ([NSNumber]) -> Void)

func deviceController(UUID, registerNodeID: NSNumber)

func deviceController(UUID, unregisterNodeID: NSNumber)

func deviceController(UUID, updateControllerConfiguration: [AnyHashable : Any])

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- MTRXPCServerProtocol

