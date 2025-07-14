

- CarPlay
-  CPInstrumentClusterControllerDelegate 

Protocol

# CPInstrumentClusterControllerDelegate

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
protocol CPInstrumentClusterControllerDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func instrumentClusterController(CPInstrumentClusterController, didChangeCompassSetting: CPInstrumentClusterSetting)

func instrumentClusterController(CPInstrumentClusterController, didChangeSpeedLimitSetting: CPInstrumentClusterSetting)

func instrumentClusterControllerDidConnect(UIWindow)

**Required**

func instrumentClusterControllerDidDisconnectWindow(UIWindow)

**Required**

func instrumentClusterControllerDidZoom(in: CPInstrumentClusterController)

func instrumentClusterControllerDidZoomOut(CPInstrumentClusterController)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Instrument cluster

class CPInstrumentClusterController

class CPTemplateApplicationInstrumentClusterScene

protocol CPTemplateApplicationInstrumentClusterSceneDelegate

