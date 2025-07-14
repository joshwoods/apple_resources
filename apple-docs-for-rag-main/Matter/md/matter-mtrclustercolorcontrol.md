

- Matter
-  MTRClusterColorControl 

Class

# MTRClusterColorControl

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterColorControl
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func colorLoopSet(with: MTRColorControlClusterColorLoopSetParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func colorLoopSet(with: MTRColorControlClusterColorLoopSetParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func enhancedMoveHue(with: MTRColorControlClusterEnhancedMoveHueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func enhancedMoveHue(with: MTRColorControlClusterEnhancedMoveHueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func enhancedMoveToHue(with: MTRColorControlClusterEnhancedMoveToHueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func enhancedMoveToHue(with: MTRColorControlClusterEnhancedMoveToHueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func enhancedMoveToHueAndSaturation(with: MTRColorControlClusterEnhancedMoveToHueAndSaturationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func enhancedMoveToHueAndSaturation(with: MTRColorControlClusterEnhancedMoveToHueAndSaturationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func enhancedStepHue(with: MTRColorControlClusterEnhancedStepHueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func enhancedStepHue(with: MTRColorControlClusterEnhancedStepHueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func moveColor(with: MTRColorControlClusterMoveColorParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func moveColor(with: MTRColorControlClusterMoveColorParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func moveColorTemperature(with: MTRColorControlClusterMoveColorTemperatureParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func moveColorTemperature(with: MTRColorControlClusterMoveColorTemperatureParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func moveHue(with: MTRColorControlClusterMoveHueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func moveHue(with: MTRColorControlClusterMoveHueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func moveSaturation(with: MTRColorControlClusterMoveSaturationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func moveSaturation(with: MTRColorControlClusterMoveSaturationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func moveToColor(with: MTRColorControlClusterMoveToColorParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func moveToColor(with: MTRColorControlClusterMoveToColorParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func moveToColorTemperature(with: MTRColorControlClusterMoveToColorTemperatureParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func moveToColorTemperature(with: MTRColorControlClusterMoveToColorTemperatureParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func moveToHue(with: MTRColorControlClusterMoveToHueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func moveToHue(with: MTRColorControlClusterMoveToHueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func moveToHueAndSaturation(with: MTRColorControlClusterMoveToHueAndSaturationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func moveToHueAndSaturation(with: MTRColorControlClusterMoveToHueAndSaturationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func moveToSaturation(with: MTRColorControlClusterMoveToSaturationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func moveToSaturation(with: MTRColorControlClusterMoveToSaturationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorCapabilities(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorLoopActive(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorLoopDirection(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorLoopStartEnhancedHue(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorLoopStoredEnhancedHue(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorLoopTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorPointBIntensity(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorPointBX(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorPointBY(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorPointGIntensity(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorPointGX(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorPointGY(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorPointRIntensity(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorPointRX(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorPointRY(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorTempPhysicalMaxMireds(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorTempPhysicalMinMireds(with: MTRReadParams?) -> [String : Any]?

func readAttributeColorTemperatureMireds(with: MTRReadParams?) -> [String : Any]?

func readAttributeCompensationText(with: MTRReadParams?) -> [String : Any]?

func readAttributeCoupleColorTempToLevelMinMireds(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentHue(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentSaturation(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentX(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentY(with: MTRReadParams?) -> [String : Any]?

func readAttributeDriftCompensation(with: MTRReadParams?) -> [String : Any]?

func readAttributeEnhancedColorMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeEnhancedCurrentHue(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfPrimaries(with: MTRReadParams?) -> [String : Any]?

func readAttributeOptions(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary1Intensity(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary1X(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary1Y(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary2Intensity(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary2X(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary2Y(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary3Intensity(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary3X(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary3Y(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary4Intensity(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary4X(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary4Y(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary5Intensity(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary5X(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary5Y(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary6Intensity(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary6X(with: MTRReadParams?) -> [String : Any]?

func readAttributePrimary6Y(with: MTRReadParams?) -> [String : Any]?

func readAttributeRemainingTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeStartUpColorTemperatureMireds(with: MTRReadParams?) -> [String : Any]?

func readAttributeWhitePointX(with: MTRReadParams?) -> [String : Any]?

func readAttributeWhitePointY(with: MTRReadParams?) -> [String : Any]?

func stepColor(with: MTRColorControlClusterStepColorParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func stepColor(with: MTRColorControlClusterStepColorParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func stepColorTemperature(with: MTRColorControlClusterStepColorTemperatureParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func stepColorTemperature(with: MTRColorControlClusterStepColorTemperatureParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func stepHue(with: MTRColorControlClusterStepHueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func stepHue(with: MTRColorControlClusterStepHueParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func stepSaturation(with: MTRColorControlClusterStepSaturationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func stepSaturation(with: MTRColorControlClusterStepSaturationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func stopMoveStep(with: MTRColorControlClusterStopMoveStepParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func stopMoveStep(with: MTRColorControlClusterStopMoveStepParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointBIntensity(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeColorPointBIntensity(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeColorPointBX(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeColorPointBX(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeColorPointBY(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeColorPointBY(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeColorPointGIntensity(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeColorPointGIntensity(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeColorPointGX(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeColorPointGX(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeColorPointGY(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeColorPointGY(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeColorPointRIntensity(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeColorPointRIntensity(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeColorPointRX(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeColorPointRX(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeColorPointRY(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeColorPointRY(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeOptions(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOptions(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeStartUpColorTemperatureMireds(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeStartUpColorTemperatureMireds(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeWhitePointX(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeWhitePointX(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeWhitePointY(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeWhitePointY(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

