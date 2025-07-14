

- Matter
-  MTRClusterThreadNetworkDiagnostics 

Class

# MTRClusterThreadNetworkDiagnostics

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterThreadNetworkDiagnostics
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveNetworkFaultsList(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveTimestamp(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttachAttemptCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeBetterPartitionAttachAttemptCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeChannel(with: MTRReadParams?) -> [String : Any]?

func readAttributeChannelPage0Mask(with: MTRReadParams?) -> [String : Any]?

func readAttributeChildRoleCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeDataVersion(with: MTRReadParams?) -> [String : Any]?

func readAttributeDelay(with: MTRReadParams?) -> [String : Any]?

func readAttributeDetachedRoleCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeExtendedPanId(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeLeaderRoleCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeLeaderRouterId(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeshLocalPrefix(with: MTRReadParams?) -> [String : Any]?

func readAttributeNeighborTable(with: MTRReadParams?) -> [String : Any]?

func readAttributeNeighborTableList(with: MTRReadParams?) -> [String : Any]Deprecated

func readAttributeNetworkName(with: MTRReadParams?) -> [String : Any]?

func readAttributeOperationalDatasetComponents(with: MTRReadParams?) -> [String : Any]?

func readAttributeOverrunCount(with: MTRReadParams?) -> [String : Any]?

func readAttributePanId(with: MTRReadParams?) -> [String : Any]?

func readAttributeParentChangeCount(with: MTRReadParams?) -> [String : Any]?

func readAttributePartitionId(with: MTRReadParams?) -> [String : Any]?

func readAttributePartitionIdChangeCount(with: MTRReadParams?) -> [String : Any]?

func readAttributePendingTimestamp(with: MTRReadParams?) -> [String : Any]?

func readAttributeRouteTable(with: MTRReadParams?) -> [String : Any]?

func readAttributeRouteTableList(with: MTRReadParams?) -> [String : Any]Deprecated

func readAttributeRouterRoleCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRoutingRole(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxAddressFilteredCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxBeaconCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxBeaconRequestCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxBroadcastCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxDataCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxDataPollCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxDestAddrFilteredCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxDuplicatedCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxErrFcsCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxErrInvalidSrcAddrCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxErrNoFrameCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxErrOtherCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxErrSecCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxErrUnknownNeighborCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxOtherCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxTotalCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRxUnicastCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeSecurityPolicy(with: MTRReadParams?) -> [String : Any]?

func readAttributeStableDataVersion(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxAckRequestedCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxAckedCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxBeaconCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxBeaconRequestCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxBroadcastCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxDataCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxDataPollCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxDirectMaxRetryExpiryCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxErrAbortCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxErrBusyChannelCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxErrCcaCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxIndirectMaxRetryExpiryCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxNoAckRequestedCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxOtherCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxRetryCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxTotalCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxUnicastCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeWeighting(with: MTRReadParams?) -> [String : Any]?

func resetCounts(with: MTRThreadNetworkDiagnosticsClusterResetCountsParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func resetCounts(with: MTRThreadNetworkDiagnosticsClusterResetCountsParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func resetCounts(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func resetCounts(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

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

