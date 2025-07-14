

- Matter
-  MTRClusterDeviceEnergyManagement 

Class

# MTRClusterDeviceEnergyManagement

Cluster Device Energy Management This cluster allows a client to manage the power draw of a device. An example of such a client could be an Energy Management System (EMS) which controls an Energy Smart Appliance (ESA).

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterDeviceEnergyManagement
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

For all instance methods that take a completion (i.e. command invocations), the completion will be called on the provided queue.

### Instance Methods

func cancelPowerAdjustRequest(with: MTRDeviceEnergyManagementClusterCancelPowerAdjustRequestParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func cancelPowerAdjustRequest(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func cancelRequest(with: MTRDeviceEnergyManagementClusterCancelRequestParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func cancelRequest(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func modifyForecastRequest(with: MTRDeviceEnergyManagementClusterModifyForecastRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func pauseRequest(with: MTRDeviceEnergyManagementClusterPauseRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func powerAdjustRequest(with: MTRDeviceEnergyManagementClusterPowerAdjustRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func readAttributeAbsMaxPower(with: MTRReadParams?) -> [String : Any]?

func readAttributeAbsMinPower(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeESACanGenerate(with: MTRReadParams?) -> [String : Any]?

func readAttributeESAState(with: MTRReadParams?) -> [String : Any]?

func readAttributeESAType(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeForecast(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeOptOutState(with: MTRReadParams?) -> [String : Any]?

func readAttributePowerAdjustmentCapability(with: MTRReadParams?) -> [String : Any]?

func requestConstraintBasedForecast(with: MTRDeviceEnergyManagementClusterRequestConstraintBasedForecastParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func resumeRequest(with: MTRDeviceEnergyManagementClusterResumeRequestParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func resumeRequest(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func startTimeAdjustRequest(with: MTRDeviceEnergyManagementClusterStartTimeAdjustRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

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

