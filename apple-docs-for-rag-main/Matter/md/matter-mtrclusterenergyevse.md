

- Matter
-  MTRClusterEnergyEVSE 

Class

# MTRClusterEnergyEVSE

Cluster Energy EVSE Electric Vehicle Supply Equipment (EVSE) is equipment used to charge an Electric Vehicle (EV) or Plug-In Hybrid Electric Vehicle. This cluster provides an interface to the functionality of Electric Vehicle Supply Equipment (EVSE) management.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterEnergyEVSE
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

For all instance methods that take a completion (i.e. command invocations), the completion will be called on the provided queue.

### Instance Methods

func clearTargets(with: MTREnergyEVSEClusterClearTargetsParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func clearTargets(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func disable(with: MTREnergyEVSEClusterDisableParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func disable(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func enableCharging(with: MTREnergyEVSEClusterEnableChargingParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func getTargetsWith(MTREnergyEVSEClusterGetTargetsParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTREnergyEVSEClusterGetTargetsResponseParams?, (any Error)?) -> Void)

func getTargetsWithExpectedValues([[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTREnergyEVSEClusterGetTargetsResponseParams?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeApproximateEVEfficiency(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeChargingEnabledUntil(with: MTRReadParams?) -> [String : Any]?

func readAttributeCircuitCapacity(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFaultState(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaximumChargeCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinimumChargeCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeNextChargeRequiredEnergy(with: MTRReadParams?) -> [String : Any]?

func readAttributeNextChargeStartTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeNextChargeTargetSoC(with: MTRReadParams?) -> [String : Any]?

func readAttributeNextChargeTargetTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeRandomizationDelayWindow(with: MTRReadParams?) -> [String : Any]?

func readAttributeSessionDuration(with: MTRReadParams?) -> [String : Any]?

func readAttributeSessionEnergyCharged(with: MTRReadParams?) -> [String : Any]?

func readAttributeSessionID(with: MTRReadParams?) -> [String : Any]?

func readAttributeState(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupplyState(with: MTRReadParams?) -> [String : Any]?

func readAttributeUserMaximumChargeCurrent(with: MTRReadParams?) -> [String : Any]?

func setTargetsWith(MTREnergyEVSEClusterSetTargetsParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func startDiagnostics(with: MTREnergyEVSEClusterStartDiagnosticsParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func startDiagnostics(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeApproximateEVEfficiency(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeApproximateEVEfficiency(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeRandomizationDelayWindow(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeRandomizationDelayWindow(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeUserMaximumChargeCurrent(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeUserMaximumChargeCurrent(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

