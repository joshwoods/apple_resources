

- Matter
-  MTRBaseClusterDeviceEnergyManagement 

Class

# MTRBaseClusterDeviceEnergyManagement

Cluster Device Energy Management

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRBaseClusterDeviceEnergyManagement
```

## Overview

This cluster allows a client to manage the power draw of a device. An example of such a client could be an Energy Management System (EMS) which controls an Energy Smart Appliance (ESA).

## Topics

### Initializers

init?(device: MTRBaseDevice, endpointID: NSNumber, queue: dispatch_queue_t)

For all instance methods (reads, writes, commands) that take a completion, the completion will be called on the provided queue.

### Instance Methods

func cancelPowerAdjustRequest(completion: MTRStatusCompletion)

func cancelPowerAdjustRequest(with: MTRDeviceEnergyManagementClusterCancelPowerAdjustRequestParams?, completion: MTRStatusCompletion)

Command CancelPowerAdjustRequest

func cancelRequest(completion: MTRStatusCompletion)

func cancelRequest(with: MTRDeviceEnergyManagementClusterCancelRequestParams?, completion: MTRStatusCompletion)

Command CancelRequest

func modifyForecastRequest(with: MTRDeviceEnergyManagementClusterModifyForecastRequestParams, completion: MTRStatusCompletion)

Command ModifyForecastRequest

func pauseRequest(with: MTRDeviceEnergyManagementClusterPauseRequestParams, completion: MTRStatusCompletion)

Command PauseRequest

func powerAdjustRequest(with: MTRDeviceEnergyManagementClusterPowerAdjustRequestParams, completion: MTRStatusCompletion)

Command PowerAdjustRequest

func readAttributeAbsMaxPower(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeAbsMinPower(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeClusterRevision(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeESACanGenerate(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeESAState(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeESAType(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeForecast(completion: (MTRDeviceEnergyManagementClusterForecastStruct?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeOptOutState(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePowerAdjustmentCapability(completion: (MTRDeviceEnergyManagementClusterPowerAdjustCapabilityStruct?, (any Error)?) -> Void)

func requestConstraintBasedForecast(with: MTRDeviceEnergyManagementClusterRequestConstraintBasedForecastParams, completion: MTRStatusCompletion)

Command RequestConstraintBasedForecast

func resumeRequest(completion: MTRStatusCompletion)

func resumeRequest(with: MTRDeviceEnergyManagementClusterResumeRequestParams?, completion: MTRStatusCompletion)

Command ResumeRequest

func startTimeAdjustRequest(with: MTRDeviceEnergyManagementClusterStartTimeAdjustRequestParams, completion: MTRStatusCompletion)

Command StartTimeAdjustRequest

func subscribeAttributeAbsMaxPower(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAbsMinPower(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeESACanGenerate(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeESAState(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeESAType(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeForecast(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (MTRDeviceEnergyManagementClusterForecastStruct?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeOptOutState(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePowerAdjustmentCapability(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (MTRDeviceEnergyManagementClusterPowerAdjustCapabilityStruct?, (any Error)?) -> Void)

### Type Methods

class func readAttributeAbsMaxPower(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAbsMinPower(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAcceptedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAttributeList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeESACanGenerate(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeESAState(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeESAType(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeForecast(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (MTRDeviceEnergyManagementClusterForecastStruct?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeOptOutState(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePowerAdjustmentCapability(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (MTRDeviceEnergyManagementClusterPowerAdjustCapabilityStruct?, (any Error)?) -> Void)

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

