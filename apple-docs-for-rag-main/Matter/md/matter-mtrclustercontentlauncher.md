

- Matter
-  MTRClusterContentLauncher 

Class

# MTRClusterContentLauncher

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterContentLauncher
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func launchContent(with: MTRContentLauncherClusterLaunchContentParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRContentLauncherClusterLauncherResponseParams?, (any Error)?) -> Void)

func launchContent(with: MTRContentLauncherClusterLaunchContentParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRContentLauncherClusterLaunchResponseParams?, (any Error)?) -> Void)Deprecated

func launchURL(with: MTRContentLauncherClusterLaunchURLParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRContentLauncherClusterLauncherResponseParams?, (any Error)?) -> Void)

func launchURL(with: MTRContentLauncherClusterLaunchURLParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRContentLauncherClusterLaunchResponseParams?, (any Error)?) -> Void)Deprecated

func readAttributeAcceptHeader(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportedStreamingProtocols(with: MTRReadParams?) -> [String : Any]?

func writeAttributeSupportedStreamingProtocols(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeSupportedStreamingProtocols(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

