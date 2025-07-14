

- Matter
-  MTRBaseClusterPowerSource 

Class

# MTRBaseClusterPowerSource

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRBaseClusterPowerSource
```

## Topics

### Initializers

init?(device: MTRBaseDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRBaseDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeActiveBatChargeFaults(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeActiveBatChargeFaults(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeActiveBatFaults(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeActiveBatFaults(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeActiveWiredFaults(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeActiveWiredFaults(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeAttributeList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeBatANSIDesignation(completion: (String?, (any Error)?) -> Void)

func readAttributeBatANSIDesignation(completionHandler: (String?, (any Error)?) -> Void)Deprecated

func readAttributeBatApprovedChemistry(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatApprovedChemistry(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBatCapacity(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatCapacity(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBatChargeLevel(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatChargeLevel(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBatChargeState(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatChargeState(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBatChargingCurrent(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatChargingCurrent(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBatCommonDesignation(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatCommonDesignation(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBatFunctionalWhileCharging(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatFunctionalWhileCharging(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBatIECDesignation(completion: (String?, (any Error)?) -> Void)

func readAttributeBatIECDesignation(completionHandler: (String?, (any Error)?) -> Void)Deprecated

func readAttributeBatPercentRemaining(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatPercentRemaining(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBatPresent(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatPresent(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBatQuantity(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatQuantity(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBatReplaceability(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatReplaceability(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBatReplacementDescription(completion: (String?, (any Error)?) -> Void)

func readAttributeBatReplacementDescription(completionHandler: (String?, (any Error)?) -> Void)Deprecated

func readAttributeBatReplacementNeeded(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatReplacementNeeded(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBatTimeRemaining(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatTimeRemaining(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBatTimeToFullCharge(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatTimeToFullCharge(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBatVoltage(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBatVoltage(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeClusterRevision(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeClusterRevision(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeDescription(completion: (String?, (any Error)?) -> Void)

func readAttributeDescription(completionHandler: (String?, (any Error)?) -> Void)Deprecated

func readAttributeEndpointList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeFeatureMap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeGeneratedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeOrder(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeOrder(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeStatus(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeStatus(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeWiredAssessedCurrent(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeWiredAssessedCurrent(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeWiredAssessedInputFrequency(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeWiredAssessedInputFrequency(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeWiredAssessedInputVoltage(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeWiredAssessedInputVoltage(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeWiredCurrentType(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeWiredCurrentType(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeWiredMaximumCurrent(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeWiredMaximumCurrent(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeWiredNominalVoltage(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeWiredNominalVoltage(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeWiredPresent(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeWiredPresent(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAcceptedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeActiveBatChargeFaults(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeActiveBatChargeFaults(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeActiveBatFaults(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeActiveBatFaults(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeActiveWiredFaults(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeActiveWiredFaults(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAttributeList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatANSIDesignation(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)

func subscribeAttributeBatANSIDesignation(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatApprovedChemistry(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatApprovedChemistry(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatCapacity(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatCapacity(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatChargeLevel(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatChargeLevel(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatChargeState(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatChargeState(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatChargingCurrent(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatChargingCurrent(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatCommonDesignation(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatCommonDesignation(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatFunctionalWhileCharging(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatFunctionalWhileCharging(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatIECDesignation(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)

func subscribeAttributeBatIECDesignation(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatPercentRemaining(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatPercentRemaining(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatPresent(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatPresent(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatQuantity(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatQuantity(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatReplaceability(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatReplaceability(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatReplacementDescription(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)

func subscribeAttributeBatReplacementDescription(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatReplacementNeeded(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatReplacementNeeded(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatTimeRemaining(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatTimeRemaining(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatTimeToFullCharge(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatTimeToFullCharge(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBatVoltage(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBatVoltage(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeClusterRevision(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeDescription(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)

func subscribeAttributeDescription(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)Deprecated

func subscribeAttributeEndpointList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeGeneratedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeOrder(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeOrder(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeStatus(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeStatus(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeWiredAssessedCurrent(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeWiredAssessedCurrent(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeWiredAssessedInputFrequency(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeWiredAssessedInputFrequency(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeWiredAssessedInputVoltage(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeWiredAssessedInputVoltage(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeWiredCurrentType(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeWiredCurrentType(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeWiredMaximumCurrent(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeWiredMaximumCurrent(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeWiredNominalVoltage(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeWiredNominalVoltage(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeWiredPresent(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeWiredPresent(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

### Type Methods

class func readAttributeAcceptedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAcceptedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeActiveBatChargeFaults(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeActiveBatChargeFaults(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeActiveBatFaults(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeActiveBatFaults(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeActiveWiredFaults(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeActiveWiredFaults(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAttributeList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAttributeList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeBatANSIDesignation(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (String?, (any Error)?) -> Void)Deprecated

class func readAttributeBatANSIDesignation(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (String?, (any Error)?) -> Void)

class func readAttributeBatApprovedChemistry(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatApprovedChemistry(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBatCapacity(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatCapacity(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBatChargeLevel(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatChargeLevel(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBatChargeState(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatChargeState(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBatChargingCurrent(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatChargingCurrent(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBatCommonDesignation(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatCommonDesignation(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBatFunctionalWhileCharging(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatFunctionalWhileCharging(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBatIECDesignation(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (String?, (any Error)?) -> Void)Deprecated

class func readAttributeBatIECDesignation(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (String?, (any Error)?) -> Void)

class func readAttributeBatPercentRemaining(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatPercentRemaining(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBatPresent(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatPresent(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBatQuantity(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatQuantity(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBatReplaceability(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatReplaceability(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBatReplacementDescription(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (String?, (any Error)?) -> Void)Deprecated

class func readAttributeBatReplacementDescription(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (String?, (any Error)?) -> Void)

class func readAttributeBatReplacementNeeded(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatReplacementNeeded(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBatTimeRemaining(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatTimeRemaining(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBatTimeToFullCharge(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatTimeToFullCharge(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBatVoltage(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBatVoltage(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeClusterRevision(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeDescription(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (String?, (any Error)?) -> Void)Deprecated

class func readAttributeDescription(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (String?, (any Error)?) -> Void)

class func readAttributeEndpointList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeFeatureMap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeGeneratedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeOrder(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeOrder(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeStatus(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeStatus(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeWiredAssessedCurrent(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeWiredAssessedCurrent(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeWiredAssessedInputFrequency(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeWiredAssessedInputFrequency(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeWiredAssessedInputVoltage(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeWiredAssessedInputVoltage(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeWiredCurrentType(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeWiredCurrentType(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeWiredMaximumCurrent(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeWiredMaximumCurrent(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeWiredNominalVoltage(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeWiredNominalVoltage(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeWiredPresent(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeWiredPresent(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

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

