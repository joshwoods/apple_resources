

- Matter
-  MTRBaseClusterColorControl 

Class

# MTRBaseClusterColorControl

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRBaseClusterColorControl
```

## Topics

### Initializers

init?(device: MTRBaseDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRBaseDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func colorLoopSet(with: MTRColorControlClusterColorLoopSetParams, completion: MTRStatusCompletion)

func colorLoopSet(with: MTRColorControlClusterColorLoopSetParams, completionHandler: MTRStatusCompletion)Deprecated

func enhancedMoveHue(with: MTRColorControlClusterEnhancedMoveHueParams, completion: MTRStatusCompletion)

func enhancedMoveHue(with: MTRColorControlClusterEnhancedMoveHueParams, completionHandler: MTRStatusCompletion)Deprecated

func enhancedMoveToHue(with: MTRColorControlClusterEnhancedMoveToHueParams, completion: MTRStatusCompletion)

func enhancedMoveToHue(with: MTRColorControlClusterEnhancedMoveToHueParams, completionHandler: MTRStatusCompletion)Deprecated

func enhancedMoveToHueAndSaturation(with: MTRColorControlClusterEnhancedMoveToHueAndSaturationParams, completion: MTRStatusCompletion)

func enhancedMoveToHueAndSaturation(with: MTRColorControlClusterEnhancedMoveToHueAndSaturationParams, completionHandler: MTRStatusCompletion)Deprecated

func enhancedStepHue(with: MTRColorControlClusterEnhancedStepHueParams, completion: MTRStatusCompletion)

func enhancedStepHue(with: MTRColorControlClusterEnhancedStepHueParams, completionHandler: MTRStatusCompletion)Deprecated

func moveColor(with: MTRColorControlClusterMoveColorParams, completion: MTRStatusCompletion)

func moveColor(with: MTRColorControlClusterMoveColorParams, completionHandler: MTRStatusCompletion)Deprecated

func moveColorTemperature(with: MTRColorControlClusterMoveColorTemperatureParams, completion: MTRStatusCompletion)

func moveColorTemperature(with: MTRColorControlClusterMoveColorTemperatureParams, completionHandler: MTRStatusCompletion)Deprecated

func moveHue(with: MTRColorControlClusterMoveHueParams, completion: MTRStatusCompletion)

func moveHue(with: MTRColorControlClusterMoveHueParams, completionHandler: MTRStatusCompletion)Deprecated

func moveSaturation(with: MTRColorControlClusterMoveSaturationParams, completion: MTRStatusCompletion)

func moveSaturation(with: MTRColorControlClusterMoveSaturationParams, completionHandler: MTRStatusCompletion)Deprecated

func moveToColor(with: MTRColorControlClusterMoveToColorParams, completion: MTRStatusCompletion)

func moveToColor(with: MTRColorControlClusterMoveToColorParams, completionHandler: MTRStatusCompletion)Deprecated

func moveToColorTemperature(with: MTRColorControlClusterMoveToColorTemperatureParams, completion: MTRStatusCompletion)

func moveToColorTemperature(with: MTRColorControlClusterMoveToColorTemperatureParams, completionHandler: MTRStatusCompletion)Deprecated

func moveToHue(with: MTRColorControlClusterMoveToHueParams, completion: MTRStatusCompletion)

func moveToHue(with: MTRColorControlClusterMoveToHueParams, completionHandler: MTRStatusCompletion)Deprecated

func moveToHueAndSaturation(with: MTRColorControlClusterMoveToHueAndSaturationParams, completion: MTRStatusCompletion)

func moveToHueAndSaturation(with: MTRColorControlClusterMoveToHueAndSaturationParams, completionHandler: MTRStatusCompletion)Deprecated

func moveToSaturation(with: MTRColorControlClusterMoveToSaturationParams, completion: MTRStatusCompletion)

func moveToSaturation(with: MTRColorControlClusterMoveToSaturationParams, completionHandler: MTRStatusCompletion)Deprecated

func readAttributeAcceptedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeAttributeList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeClusterRevision(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeClusterRevision(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorCapabilities(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorCapabilities(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorLoopActive(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorLoopActive(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorLoopDirection(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorLoopDirection(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorLoopStartEnhancedHue(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorLoopStartEnhancedHue(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorLoopStoredEnhancedHue(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorLoopStoredEnhancedHue(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorLoopTime(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorLoopTime(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorMode(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorMode(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorPointBIntensity(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorPointBIntensity(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorPointBX(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorPointBX(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorPointBY(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorPointBY(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorPointGIntensity(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorPointGIntensity(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorPointGX(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorPointGX(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorPointGY(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorPointGY(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorPointRIntensity(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorPointRIntensity(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorPointRX(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorPointRX(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorPointRY(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorPointRY(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorTempPhysicalMaxMireds(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorTempPhysicalMaxMireds(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorTempPhysicalMinMireds(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorTempPhysicalMinMireds(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeColorTemperatureMireds(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeColorTemperatureMireds(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeCompensationText(completion: (String?, (any Error)?) -> Void)

func readAttributeCompensationText(completionHandler: (String?, (any Error)?) -> Void)Deprecated

func readAttributeCoupleColorTempToLevelMinMireds(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeCoupleColorTempToLevelMinMireds(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeCurrentHue(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeCurrentHue(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeCurrentSaturation(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeCurrentSaturation(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeCurrentX(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeCurrentX(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeCurrentY(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeCurrentY(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeDriftCompensation(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeDriftCompensation(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeEnhancedColorMode(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeEnhancedColorMode(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeEnhancedCurrentHue(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeEnhancedCurrentHue(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeFeatureMap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeGeneratedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeNumberOfPrimaries(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNumberOfPrimaries(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeOptions(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeOptions(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary1Intensity(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary1Intensity(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary1X(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary1X(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary1Y(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary1Y(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary2Intensity(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary2Intensity(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary2X(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary2X(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary2Y(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary2Y(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary3Intensity(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary3Intensity(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary3X(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary3X(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary3Y(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary3Y(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary4Intensity(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary4Intensity(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary4X(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary4X(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary4Y(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary4Y(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary5Intensity(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary5Intensity(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary5X(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary5X(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary5Y(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary5Y(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary6Intensity(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary6Intensity(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary6X(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary6X(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePrimary6Y(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePrimary6Y(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeRemainingTime(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeRemainingTime(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeStartUpColorTemperatureMireds(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeStartUpColorTemperatureMireds(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeWhitePointX(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeWhitePointX(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeWhitePointY(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeWhitePointY(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func stepColor(with: MTRColorControlClusterStepColorParams, completion: MTRStatusCompletion)

func stepColor(with: MTRColorControlClusterStepColorParams, completionHandler: MTRStatusCompletion)Deprecated

func stepColorTemperature(with: MTRColorControlClusterStepColorTemperatureParams, completion: MTRStatusCompletion)

func stepColorTemperature(with: MTRColorControlClusterStepColorTemperatureParams, completionHandler: MTRStatusCompletion)Deprecated

func stepHue(with: MTRColorControlClusterStepHueParams, completion: MTRStatusCompletion)

func stepHue(with: MTRColorControlClusterStepHueParams, completionHandler: MTRStatusCompletion)Deprecated

func stepSaturation(with: MTRColorControlClusterStepSaturationParams, completion: MTRStatusCompletion)

func stepSaturation(with: MTRColorControlClusterStepSaturationParams, completionHandler: MTRStatusCompletion)Deprecated

func stopMoveStep(with: MTRColorControlClusterStopMoveStepParams, completion: MTRStatusCompletion)

func stopMoveStep(with: MTRColorControlClusterStopMoveStepParams, completionHandler: MTRStatusCompletion)Deprecated

func subscribeAttributeAcceptedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAttributeList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeClusterRevision(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorCapabilities(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorCapabilities(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorLoopActive(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorLoopActive(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorLoopDirection(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorLoopDirection(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorLoopStartEnhancedHue(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorLoopStartEnhancedHue(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorLoopStoredEnhancedHue(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorLoopStoredEnhancedHue(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorLoopTime(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorLoopTime(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorMode(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorMode(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorPointBIntensity(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorPointBIntensity(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorPointBX(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorPointBX(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorPointBY(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorPointBY(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorPointGIntensity(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorPointGIntensity(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorPointGX(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorPointGX(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorPointGY(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorPointGY(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorPointRIntensity(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorPointRIntensity(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorPointRX(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorPointRX(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorPointRY(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorPointRY(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorTempPhysicalMaxMireds(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorTempPhysicalMaxMireds(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorTempPhysicalMinMireds(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorTempPhysicalMinMireds(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeColorTemperatureMireds(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeColorTemperatureMireds(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeCompensationText(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)

func subscribeAttributeCompensationText(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)Deprecated

func subscribeAttributeCoupleColorTempToLevelMinMireds(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeCoupleColorTempToLevelMinMireds(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeCurrentHue(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeCurrentHue(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeCurrentSaturation(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeCurrentSaturation(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeCurrentX(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeCurrentX(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeCurrentY(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeCurrentY(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeDriftCompensation(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeDriftCompensation(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeEnhancedColorMode(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEnhancedColorMode(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeEnhancedCurrentHue(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEnhancedCurrentHue(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeFeatureMap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeGeneratedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeNumberOfPrimaries(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNumberOfPrimaries(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeOptions(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeOptions(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary1Intensity(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary1Intensity(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary1X(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary1X(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary1Y(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary1Y(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary2Intensity(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary2Intensity(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary2X(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary2X(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary2Y(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary2Y(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary3Intensity(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary3Intensity(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary3X(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary3X(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary3Y(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary3Y(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary4Intensity(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary4Intensity(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary4X(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary4X(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary4Y(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary4Y(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary5Intensity(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary5Intensity(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary5X(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary5X(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary5Y(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary5Y(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary6Intensity(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary6Intensity(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary6X(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary6X(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePrimary6Y(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePrimary6Y(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeRemainingTime(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeRemainingTime(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeStartUpColorTemperatureMireds(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeStartUpColorTemperatureMireds(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeWhitePointX(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeWhitePointX(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeWhitePointY(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeWhitePointY(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func writeAttributeColorPointBIntensity(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeColorPointBIntensity(withValue: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointBIntensity(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeColorPointBIntensity(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointBX(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeColorPointBX(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointBX(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeColorPointBX(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointBY(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeColorPointBY(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointBY(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeColorPointBY(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointGIntensity(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeColorPointGIntensity(withValue: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointGIntensity(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeColorPointGIntensity(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointGX(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeColorPointGX(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointGX(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeColorPointGX(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointGY(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeColorPointGY(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointGY(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeColorPointGY(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointRIntensity(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeColorPointRIntensity(withValue: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointRIntensity(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeColorPointRIntensity(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointRX(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeColorPointRX(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointRX(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeColorPointRX(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointRY(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeColorPointRY(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeColorPointRY(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeColorPointRY(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeOptions(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeOptions(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeOptions(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeOptions(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeStartUpColorTemperatureMireds(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeStartUpColorTemperatureMireds(withValue: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeStartUpColorTemperatureMireds(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeStartUpColorTemperatureMireds(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeWhitePointX(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeWhitePointX(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeWhitePointX(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeWhitePointX(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeWhitePointY(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeWhitePointY(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeWhitePointY(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeWhitePointY(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

### Type Methods

class func readAttributeAcceptedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAcceptedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAttributeList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAttributeList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeClusterRevision(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorCapabilities(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorCapabilities(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorLoopActive(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorLoopActive(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorLoopDirection(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorLoopDirection(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorLoopStartEnhancedHue(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorLoopStartEnhancedHue(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorLoopStoredEnhancedHue(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorLoopStoredEnhancedHue(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorLoopTime(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorLoopTime(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorMode(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorMode(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorPointBIntensity(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorPointBIntensity(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorPointBX(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorPointBX(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorPointBY(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorPointBY(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorPointGIntensity(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorPointGIntensity(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorPointGX(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorPointGX(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorPointGY(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorPointGY(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorPointRIntensity(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorPointRIntensity(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorPointRX(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorPointRX(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorPointRY(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorPointRY(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorTempPhysicalMaxMireds(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorTempPhysicalMaxMireds(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorTempPhysicalMinMireds(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorTempPhysicalMinMireds(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeColorTemperatureMireds(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeColorTemperatureMireds(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeCompensationText(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (String?, (any Error)?) -> Void)Deprecated

class func readAttributeCompensationText(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (String?, (any Error)?) -> Void)

class func readAttributeCoupleColorTempToLevelMinMireds(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeCoupleColorTempToLevelMinMireds(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeCurrentHue(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeCurrentHue(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeCurrentSaturation(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeCurrentSaturation(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeCurrentX(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeCurrentX(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeCurrentY(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeCurrentY(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeDriftCompensation(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeDriftCompensation(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEnhancedColorMode(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeEnhancedColorMode(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEnhancedCurrentHue(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeEnhancedCurrentHue(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeFeatureMap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeGeneratedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeNumberOfPrimaries(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeNumberOfPrimaries(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeOptions(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeOptions(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary1Intensity(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary1Intensity(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary1X(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary1X(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary1Y(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary1Y(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary2Intensity(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary2Intensity(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary2X(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary2X(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary2Y(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary2Y(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary3Intensity(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary3Intensity(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary3X(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary3X(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary3Y(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary3Y(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary4Intensity(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary4Intensity(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary4X(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary4X(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary4Y(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary4Y(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary5Intensity(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary5Intensity(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary5X(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary5X(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary5Y(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary5Y(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary6Intensity(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary6Intensity(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary6X(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary6X(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePrimary6Y(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePrimary6Y(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeRemainingTime(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeRemainingTime(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeStartUpColorTemperatureMireds(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeStartUpColorTemperatureMireds(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeWhitePointX(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeWhitePointX(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeWhitePointY(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeWhitePointY(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

## Relationships

### Inherits From

- MTRGenericBaseCluster

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

