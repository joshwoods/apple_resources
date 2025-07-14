

- Matter
-  MTROTAProviderDelegate 

Protocol

# MTROTAProviderDelegate

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.1+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol MTROTAProviderDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func handleApplyUpdateRequest(forNodeID: NSNumber, controller: MTRDeviceController, params: MTROTASoftwareUpdateProviderClusterApplyUpdateRequestParams, completion: (MTROTASoftwareUpdateProviderClusterApplyUpdateResponseParams?, (any Error)?) -> Void)

func handleApplyUpdateRequest(forNodeID: NSNumber, controller: MTRDeviceController, params: MTROtaSoftwareUpdateProviderClusterApplyUpdateRequestParams, completionHandler: (MTROtaSoftwareUpdateProviderClusterApplyUpdateResponseParams?, (any Error)?) -> Void)Deprecated

func handleBDXQuery(forNodeID: NSNumber, controller: MTRDeviceController, blockSize: NSNumber, blockIndex: NSNumber, bytesToSkip: NSNumber, completion: (Data?, Bool) -> Void)

func handleBDXQuery(forNodeID: NSNumber, controller: MTRDeviceController, blockSize: NSNumber, blockIndex: NSNumber, bytesToSkip: NSNumber, completionHandler: (Data?, Bool) -> Void)Deprecated

func handleBDXTransferSessionBegin(forNodeID: NSNumber, controller: MTRDeviceController, fileDesignator: String, offset: NSNumber, completion: MTRStatusCompletion)

func handleBDXTransferSessionBegin(forNodeID: NSNumber, controller: MTRDeviceController, fileDesignator: String, offset: NSNumber, completionHandler: StatusCompletion)Deprecated

func handleBDXTransferSessionEnd(forNodeID: NSNumber, controller: MTRDeviceController, error: (any Error)?)

func handleNotifyUpdateApplied(forNodeID: NSNumber, controller: MTRDeviceController, params: MTROTASoftwareUpdateProviderClusterNotifyUpdateAppliedParams, completion: MTRStatusCompletion)

func handleNotifyUpdateApplied(forNodeID: NSNumber, controller: MTRDeviceController, params: MTROtaSoftwareUpdateProviderClusterNotifyUpdateAppliedParams, completionHandler: StatusCompletion)Deprecated

func handleQueryImage(forNodeID: NSNumber, controller: MTRDeviceController, params: MTROTASoftwareUpdateProviderClusterQueryImageParams, completion: (MTROTASoftwareUpdateProviderClusterQueryImageResponseParams?, (any Error)?) -> Void)

func handleQueryImage(forNodeID: NSNumber, controller: MTRDeviceController, params: MTROtaSoftwareUpdateProviderClusterQueryImageParams, completionHandler: (MTROtaSoftwareUpdateProviderClusterQueryImageResponseParams?, (any Error)?) -> Void)Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

