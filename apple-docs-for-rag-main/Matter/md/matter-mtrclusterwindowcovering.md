

- Matter
-  MTRClusterWindowCovering 

Class

# MTRClusterWindowCovering

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterWindowCovering
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func downOrClose(with: MTRWindowCoveringClusterDownOrCloseParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func downOrClose(with: MTRWindowCoveringClusterDownOrCloseParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func downOrClose(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func downOrClose(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func goToLiftPercentage(with: MTRWindowCoveringClusterGoToLiftPercentageParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func goToLiftPercentage(with: MTRWindowCoveringClusterGoToLiftPercentageParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func goToLiftValue(with: MTRWindowCoveringClusterGoToLiftValueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func goToLiftValue(with: MTRWindowCoveringClusterGoToLiftValueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func goToTiltPercentage(with: MTRWindowCoveringClusterGoToTiltPercentageParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func goToTiltPercentage(with: MTRWindowCoveringClusterGoToTiltPercentageParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func goToTiltValue(with: MTRWindowCoveringClusterGoToTiltValueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func goToTiltValue(with: MTRWindowCoveringClusterGoToTiltValueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeConfigStatus(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentPositionLift(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentPositionLiftPercent100ths(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentPositionLiftPercentage(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentPositionTilt(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentPositionTiltPercent100ths(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentPositionTiltPercentage(with: MTRReadParams?) -> [String : Any]?

func readAttributeEndProductType(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeInstalledClosedLimitLift(with: MTRReadParams?) -> [String : Any]?

func readAttributeInstalledClosedLimitTilt(with: MTRReadParams?) -> [String : Any]?

func readAttributeInstalledOpenLimitLift(with: MTRReadParams?) -> [String : Any]?

func readAttributeInstalledOpenLimitTilt(with: MTRReadParams?) -> [String : Any]?

func readAttributeMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfActuationsLift(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfActuationsTilt(with: MTRReadParams?) -> [String : Any]?

func readAttributeOperationalStatus(with: MTRReadParams?) -> [String : Any]?

func readAttributePhysicalClosedLimitLift(with: MTRReadParams?) -> [String : Any]?

func readAttributePhysicalClosedLimitTilt(with: MTRReadParams?) -> [String : Any]?

func readAttributeSafetyStatus(with: MTRReadParams?) -> [String : Any]?

func readAttributeTargetPositionLiftPercent100ths(with: MTRReadParams?) -> [String : Any]?

func readAttributeTargetPositionTiltPercent100ths(with: MTRReadParams?) -> [String : Any]?

func readAttributeType(with: MTRReadParams?) -> [String : Any]?

func stopMotion(with: MTRWindowCoveringClusterStopMotionParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func stopMotion(with: MTRWindowCoveringClusterStopMotionParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func stopMotion(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func stopMotion(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func upOrOpen(with: MTRWindowCoveringClusterUpOrOpenParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func upOrOpen(with: MTRWindowCoveringClusterUpOrOpenParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func upOrOpen(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func upOrOpen(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMode(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeMode(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

