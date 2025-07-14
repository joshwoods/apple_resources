

- Matter
-  MTRBaseClusterTestCluster Deprecated

Class

# MTRBaseClusterTestCluster

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
class MTRBaseClusterTestCluster
```

Deprecated

Please use MTRBaseClusterUnitTesting

## Topics

### Initializers

init?(device: MTRBaseDevice, endpoint: UInt16, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeBitmap16(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeBitmap32(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeBitmap64(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeBitmap8(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeBoolean(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeCharString(completionHandler: (String?, (any Error)?) -> Void)

func readAttributeClusterErrorBoolean(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeClusterRevision(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeEnum16(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeEnum8(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeEnumAttr(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeEpochS(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeEpochUs(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeFloatDouble(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeFloatSingle(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeGeneralErrorBoolean(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeInt16s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt16u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt24s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt24u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt32s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt32u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt40s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt40u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt48s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt48u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt56s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt56u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt64s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt64u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt8s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt8u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeListFabricScoped(with: MTRReadParams?, completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeListInt8u(completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeListLongOctetString(completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeListNullablesAndOptionalsStruct(completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeListOctetString(completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeListStructOctetString(completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeLongCharString(completionHandler: (String?, (any Error)?) -> Void)

func readAttributeLongOctetString(completionHandler: (Data?, (any Error)?) -> Void)

func readAttributeNullableBitmap16(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableBitmap32(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableBitmap64(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableBitmap8(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableBoolean(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableCharString(completionHandler: (String?, (any Error)?) -> Void)

func readAttributeNullableEnum16(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableEnum8(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableEnumAttr(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableFloatDouble(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableFloatSingle(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt16s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt16u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt24s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt24u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt32s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt32u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt40s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt40u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt48s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt48u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt56s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt56u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt64s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt64u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt8s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt8u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableOctetString(completionHandler: (Data?, (any Error)?) -> Void)

func readAttributeNullableRangeRestrictedInt16s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableRangeRestrictedInt16u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableRangeRestrictedInt8s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableRangeRestrictedInt8u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableStruct(completionHandler: (MTRTestClusterClusterSimpleStruct?, (any Error)?) -> Void)

func readAttributeOctetString(completionHandler: (Data?, (any Error)?) -> Void)

func readAttributeRangeRestrictedInt16s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeRangeRestrictedInt16u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeRangeRestrictedInt8s(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeRangeRestrictedInt8u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeStructAttr(completionHandler: (MTRTestClusterClusterSimpleStruct?, (any Error)?) -> Void)

func readAttributeTimedWriteBoolean(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeUnsupported(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeVendorId(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeWriteOnlyInt8u(completionHandler: (NSNumber?, (any Error)?) -> Void)

func simpleStructEchoRequest(with: MTRTestClusterClusterSimpleStructEchoRequestParams, completionHandler: (MTRTestClusterClusterSimpleStructResponseParams?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeBitmap16(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBitmap32(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBitmap64(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBitmap8(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBoolean(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeCharString(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)

func subscribeAttributeClusterErrorBoolean(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEnum16(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEnum8(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEnumAttr(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEpochS(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEpochUs(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFloatDouble(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFloatSingle(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeGeneralErrorBoolean(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeInt16s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt16u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt24s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt24u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt32s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt32u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt40s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt40u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt48s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt48u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt56s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt56u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt64s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt64u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt8s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt8u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeListFabricScoped(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeListInt8u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeListLongOctetString(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeListNullablesAndOptionalsStruct(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeListOctetString(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeListStructOctetString(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeLongCharString(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)

func subscribeAttributeLongOctetString(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (Data?, (any Error)?) -> Void)

func subscribeAttributeNullableBitmap16(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableBitmap32(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableBitmap64(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableBitmap8(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableBoolean(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableCharString(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)

func subscribeAttributeNullableEnum16(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableEnum8(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableEnumAttr(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableFloatDouble(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableFloatSingle(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt16s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt16u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt24s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt24u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt32s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt32u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt40s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt40u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt48s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt48u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt56s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt56u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt64s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt64u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt8s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt8u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableOctetString(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (Data?, (any Error)?) -> Void)

func subscribeAttributeNullableRangeRestrictedInt16s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableRangeRestrictedInt16u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableRangeRestrictedInt8s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableRangeRestrictedInt8u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableStruct(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (MTRTestClusterClusterSimpleStruct?, (any Error)?) -> Void)

func subscribeAttributeOctetString(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (Data?, (any Error)?) -> Void)

func subscribeAttributeRangeRestrictedInt16s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeRangeRestrictedInt16u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeRangeRestrictedInt8s(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeRangeRestrictedInt8u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeStructAttr(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (MTRTestClusterClusterSimpleStruct?, (any Error)?) -> Void)

func subscribeAttributeTimedWriteBoolean(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeUnsupported(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeVendorId(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeWriteOnlyInt8u(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func test(completionHandler: MTRStatusCompletion)

func test(with: MTRTestClusterClusterTestParams?, completionHandler: MTRStatusCompletion)

func testAddArguments(with: MTRTestClusterClusterTestAddArgumentsParams, completionHandler: (MTRTestClusterClusterTestAddArgumentsResponseParams?, (any Error)?) -> Void)

func testComplexNullableOptionalRequest(with: MTRTestClusterClusterTestComplexNullableOptionalRequestParams, completionHandler: (MTRTestClusterClusterTestComplexNullableOptionalResponseParams?, (any Error)?) -> Void)

func testEmitTestEventRequest(with: MTRTestClusterClusterTestEmitTestEventRequestParams, completionHandler: (MTRTestClusterClusterTestEmitTestEventResponseParams?, (any Error)?) -> Void)

func testEmitTestFabricScopedEventRequest(with: MTRTestClusterClusterTestEmitTestFabricScopedEventRequestParams, completionHandler: (MTRTestClusterClusterTestEmitTestFabricScopedEventResponseParams?, (any Error)?) -> Void)

func testEnumsRequest(with: MTRTestClusterClusterTestEnumsRequestParams, completionHandler: (MTRTestClusterClusterTestEnumsResponseParams?, (any Error)?) -> Void)

func testListInt8UArgumentRequest(with: MTRTestClusterClusterTestListInt8UArgumentRequestParams, completionHandler: (MTRTestClusterClusterBooleanResponseParams?, (any Error)?) -> Void)

func testListInt8UReverseRequest(with: MTRTestClusterClusterTestListInt8UReverseRequestParams, completionHandler: (MTRTestClusterClusterTestListInt8UReverseResponseParams?, (any Error)?) -> Void)

func testListNestedStructListArgumentRequest(with: MTRTestClusterClusterTestListNestedStructListArgumentRequestParams, completionHandler: (MTRTestClusterClusterBooleanResponseParams?, (any Error)?) -> Void)

func testListStructArgumentRequest(with: MTRTestClusterClusterTestListStructArgumentRequestParams, completionHandler: (MTRTestClusterClusterBooleanResponseParams?, (any Error)?) -> Void)

func testNestedStructArgumentRequest(with: MTRTestClusterClusterTestNestedStructArgumentRequestParams, completionHandler: (MTRTestClusterClusterBooleanResponseParams?, (any Error)?) -> Void)

func testNestedStructListArgumentRequest(with: MTRTestClusterClusterTestNestedStructListArgumentRequestParams, completionHandler: (MTRTestClusterClusterBooleanResponseParams?, (any Error)?) -> Void)

func testNotHandled(completionHandler: MTRStatusCompletion)

func testNotHandled(with: MTRTestClusterClusterTestNotHandledParams?, completionHandler: MTRStatusCompletion)

func testNullableOptionalRequest(completionHandler: (MTRTestClusterClusterTestNullableOptionalResponseParams?, (any Error)?) -> Void)

func testNullableOptionalRequest(with: MTRTestClusterClusterTestNullableOptionalRequestParams?, completionHandler: (MTRTestClusterClusterTestNullableOptionalResponseParams?, (any Error)?) -> Void)

func testSimpleArgumentRequest(with: MTRTestClusterClusterTestSimpleArgumentRequestParams, completionHandler: (MTRTestClusterClusterTestSimpleArgumentResponseParams?, (any Error)?) -> Void)

func testSimpleOptionalArgumentRequest(completionHandler: MTRStatusCompletion)

func testSimpleOptionalArgumentRequest(with: MTRTestClusterClusterTestSimpleOptionalArgumentRequestParams?, completionHandler: MTRStatusCompletion)

func testSpecific(completionHandler: (MTRTestClusterClusterTestSpecificResponseParams?, (any Error)?) -> Void)

func testSpecific(with: MTRTestClusterClusterTestSpecificParams?, completionHandler: (MTRTestClusterClusterTestSpecificResponseParams?, (any Error)?) -> Void)

func testStructArgumentRequest(with: MTRTestClusterClusterTestStructArgumentRequestParams, completionHandler: (MTRTestClusterClusterBooleanResponseParams?, (any Error)?) -> Void)

func testStructArrayArgumentRequest(with: MTRTestClusterClusterTestStructArrayArgumentRequestParams, completionHandler: (MTRTestClusterClusterTestStructArrayArgumentResponseParams?, (any Error)?) -> Void)

func testUnknownCommand(completionHandler: MTRStatusCompletion)

func testUnknownCommand(with: MTRTestClusterClusterTestUnknownCommandParams?, completionHandler: MTRStatusCompletion)

func timedInvokeRequest(completionHandler: MTRStatusCompletion)

func timedInvokeRequest(with: MTRTestClusterClusterTimedInvokeRequestParams?, completionHandler: MTRStatusCompletion)

func writeAttributeBitmap16(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeBitmap16(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeBitmap32(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeBitmap32(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeBitmap64(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeBitmap64(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeBitmap8(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeBitmap8(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeBoolean(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeBoolean(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeCharString(withValue: String, completionHandler: MTRStatusCompletion)

func writeAttributeCharString(withValue: String, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeClusterErrorBoolean(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeClusterErrorBoolean(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeEnum16(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeEnum16(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeEnum8(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeEnum8(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeEnumAttr(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeEnumAttr(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeEpochS(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeEpochS(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeEpochUs(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeEpochUs(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeFloatDouble(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeFloatDouble(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeFloatSingle(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeFloatSingle(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeGeneralErrorBoolean(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeGeneralErrorBoolean(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt16s(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt16s(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt16u(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt16u(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt24s(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt24s(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt24u(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt24u(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt32s(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt32s(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt32u(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt32u(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt40s(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt40s(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt40u(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt40u(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt48s(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt48s(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt48u(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt48u(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt56s(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt56s(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt56u(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt56u(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt64s(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt64s(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt64u(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt64u(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt8s(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt8s(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeInt8u(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeInt8u(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeListFabricScoped(withValue: [Any], completionHandler: MTRStatusCompletion)

func writeAttributeListFabricScoped(withValue: [Any], params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeListInt8u(withValue: [Any], completionHandler: MTRStatusCompletion)

func writeAttributeListInt8u(withValue: [Any], params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeListLongOctetString(withValue: [Any], completionHandler: MTRStatusCompletion)

func writeAttributeListLongOctetString(withValue: [Any], params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeListNullablesAndOptionalsStruct(withValue: [Any], completionHandler: MTRStatusCompletion)

func writeAttributeListNullablesAndOptionalsStruct(withValue: [Any], params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeListOctetString(withValue: [Any], completionHandler: MTRStatusCompletion)

func writeAttributeListOctetString(withValue: [Any], params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeListStructOctetString(withValue: [Any], completionHandler: MTRStatusCompletion)

func writeAttributeListStructOctetString(withValue: [Any], params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeLongCharString(withValue: String, completionHandler: MTRStatusCompletion)

func writeAttributeLongCharString(withValue: String, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeLongOctetString(withValue: Data, completionHandler: MTRStatusCompletion)

func writeAttributeLongOctetString(withValue: Data, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableBitmap16(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableBitmap16(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableBitmap32(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableBitmap32(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableBitmap64(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableBitmap64(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableBitmap8(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableBitmap8(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableBoolean(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableBoolean(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableCharString(withValue: String?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableCharString(withValue: String?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableEnum16(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableEnum16(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableEnum8(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableEnum8(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableEnumAttr(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableEnumAttr(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableFloatDouble(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableFloatDouble(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableFloatSingle(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableFloatSingle(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt16s(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt16s(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt16u(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt16u(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt24s(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt24s(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt24u(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt24u(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt32s(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt32s(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt32u(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt32u(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt40s(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt40s(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt40u(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt40u(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt48s(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt48s(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt48u(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt48u(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt56s(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt56s(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt56u(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt56u(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt64s(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt64s(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt64u(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt64u(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt8s(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt8s(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt8u(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableInt8u(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableOctetString(withValue: Data?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableOctetString(withValue: Data?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt16s(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt16s(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt16u(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt16u(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt8s(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt8s(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt8u(withValue: NSNumber?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt8u(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableStruct(withValue: MTRTestClusterClusterSimpleStruct?, completionHandler: MTRStatusCompletion)

func writeAttributeNullableStruct(withValue: MTRTestClusterClusterSimpleStruct?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeOctetString(withValue: Data, completionHandler: MTRStatusCompletion)

func writeAttributeOctetString(withValue: Data, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt16s(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt16s(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt16u(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt16u(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt8s(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt8s(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt8u(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt8u(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeStructAttr(withValue: MTRTestClusterClusterSimpleStruct, completionHandler: MTRStatusCompletion)

func writeAttributeStructAttr(withValue: MTRTestClusterClusterSimpleStruct, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeTimedWriteBoolean(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeTimedWriteBoolean(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeUnsupported(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeUnsupported(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeVendorId(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeVendorId(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeWriteOnlyInt8u(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeWriteOnlyInt8u(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

### Type Methods

class func readAttributeAcceptedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeAttributeList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeBitmap16(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBitmap32(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBitmap64(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBitmap8(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBoolean(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeCharString(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (String?, (any Error)?) -> Void)

class func readAttributeClusterErrorBoolean(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEnum16(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEnum8(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEnumAttr(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEpochS(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEpochUs(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFloatDouble(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFloatSingle(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneralErrorBoolean(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeInt16s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt16u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt24s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt24u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt32s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt32u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt40s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt40u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt48s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt48u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt56s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt56u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt64s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt64u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt8s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt8u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeListFabricScoped(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeListInt8u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeListLongOctetString(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeListNullablesAndOptionalsStruct(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeListOctetString(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeListStructOctetString(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeLongCharString(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (String?, (any Error)?) -> Void)

class func readAttributeLongOctetString(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (Data?, (any Error)?) -> Void)

class func readAttributeNullableBitmap16(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableBitmap32(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableBitmap64(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableBitmap8(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableBoolean(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableCharString(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (String?, (any Error)?) -> Void)

class func readAttributeNullableEnum16(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableEnum8(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableEnumAttr(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableFloatDouble(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableFloatSingle(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt16s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt16u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt24s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt24u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt32s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt32u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt40s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt40u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt48s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt48u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt56s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt56u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt64s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt64u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt8s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt8u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableOctetString(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (Data?, (any Error)?) -> Void)

class func readAttributeNullableRangeRestrictedInt16s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableRangeRestrictedInt16u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableRangeRestrictedInt8s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableRangeRestrictedInt8u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableStruct(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (MTRTestClusterClusterSimpleStruct?, (any Error)?) -> Void)

class func readAttributeOctetString(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (Data?, (any Error)?) -> Void)

class func readAttributeRangeRestrictedInt16s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeRangeRestrictedInt16u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeRangeRestrictedInt8s(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeRangeRestrictedInt8u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeStructAttr(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (MTRTestClusterClusterSimpleStruct?, (any Error)?) -> Void)

class func readAttributeTimedWriteBoolean(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeUnsupported(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeVendorId(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeWriteOnlyInt8u(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

## Relationships

### Inherits From

- MTRBaseClusterUnitTesting

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

