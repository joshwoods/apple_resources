

- Matter
-  MTRClusterApplicationLauncher 

Class

# MTRClusterApplicationLauncher

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterApplicationLauncher
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func hideApp(with: MTRApplicationLauncherClusterHideAppParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRApplicationLauncherClusterLauncherResponseParams?, (any Error)?) -> Void)

func hideApp(with: MTRApplicationLauncherClusterHideAppParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRApplicationLauncherClusterLauncherResponseParams?, (any Error)?) -> Void)Deprecated

func hideApp(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRApplicationLauncherClusterLauncherResponseParams?, (any Error)?) -> Void)

func launchApp(with: MTRApplicationLauncherClusterLaunchAppParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRApplicationLauncherClusterLauncherResponseParams?, (any Error)?) -> Void)

func launchApp(with: MTRApplicationLauncherClusterLaunchAppParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRApplicationLauncherClusterLauncherResponseParams?, (any Error)?) -> Void)Deprecated

func launchApp(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRApplicationLauncherClusterLauncherResponseParams?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeCatalogList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentApp(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func stopApp(with: MTRApplicationLauncherClusterStopAppParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRApplicationLauncherClusterLauncherResponseParams?, (any Error)?) -> Void)

func stopApp(with: MTRApplicationLauncherClusterStopAppParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRApplicationLauncherClusterLauncherResponseParams?, (any Error)?) -> Void)Deprecated

func stopApp(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRApplicationLauncherClusterLauncherResponseParams?, (any Error)?) -> Void)

func writeAttributeCurrentApp(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeCurrentApp(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

## Relationships

### Inherits From

- MTRGenericCluster

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

