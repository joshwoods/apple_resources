

- Matter
-  MTRBaseClusterUnitTesting 

Class

# MTRBaseClusterUnitTesting

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class MTRBaseClusterUnitTesting
```

## Topics

### Initializers

init?(device: MTRBaseDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeBitmap16(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBitmap32(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBitmap64(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBitmap8(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBoolean(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeCharString(completion: (String?, (any Error)?) -> Void)

func readAttributeClusterErrorBoolean(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeClusterRevision(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeEnum16(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeEnum8(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeEnumAttr(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeEpochS(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeEpochUs(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFloatDouble(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFloatSingle(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeGeneralErrorBoolean(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeInt16s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt16u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt24s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt24u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt32s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt32u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt40s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt40u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt48s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt48u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt56s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt56u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt64s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt64u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt8s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInt8u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeListFabricScoped(with: MTRReadParams?, completion: ([Any]?, (any Error)?) -> Void)

func readAttributeListInt8u(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeListLongOctetString(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeListNullablesAndOptionalsStruct(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeListOctetString(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeListStructOctetString(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeLongCharString(completion: (String?, (any Error)?) -> Void)

func readAttributeLongOctetString(completion: (Data?, (any Error)?) -> Void)

func readAttributeNullableBitmap16(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableBitmap32(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableBitmap64(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableBitmap8(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableBoolean(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableCharString(completion: (String?, (any Error)?) -> Void)

func readAttributeNullableEnum16(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableEnum8(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableEnumAttr(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableFloatDouble(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableFloatSingle(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt16s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt16u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt24s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt24u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt32s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt32u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt40s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt40u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt48s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt48u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt56s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt56u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt64s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt64u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt8s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableInt8u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableOctetString(completion: (Data?, (any Error)?) -> Void)

func readAttributeNullableRangeRestrictedInt16s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableRangeRestrictedInt16u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableRangeRestrictedInt8s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableRangeRestrictedInt8u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNullableStruct(completion: (MTRUnitTestingClusterSimpleStruct?, (any Error)?) -> Void)

func readAttributeOctetString(completion: (Data?, (any Error)?) -> Void)

func readAttributeRangeRestrictedInt16s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeRangeRestrictedInt16u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeRangeRestrictedInt8s(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeRangeRestrictedInt8u(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeStructAttr(completion: (MTRUnitTestingClusterSimpleStruct?, (any Error)?) -> Void)

func readAttributeTimedWriteBoolean(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeUnsupported(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeVendorId(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeWriteOnlyInt8u(completion: (NSNumber?, (any Error)?) -> Void)

func simpleStructEchoRequest(with: MTRUnitTestingClusterSimpleStructEchoRequestParams, completion: (MTRUnitTestingClusterSimpleStructResponseParams?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeBitmap16(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBitmap32(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBitmap64(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBitmap8(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBoolean(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeCharString(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)

func subscribeAttributeClusterErrorBoolean(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEnum16(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEnum8(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEnumAttr(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEpochS(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEpochUs(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFloatDouble(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFloatSingle(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeGeneralErrorBoolean(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeInt16s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt16u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt24s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt24u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt32s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt32u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt40s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt40u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt48s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt48u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt56s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt56u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt64s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt64u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt8s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInt8u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeListFabricScoped(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeListInt8u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeListLongOctetString(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeListNullablesAndOptionalsStruct(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeListOctetString(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeListStructOctetString(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeLongCharString(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)

func subscribeAttributeLongOctetString(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (Data?, (any Error)?) -> Void)

func subscribeAttributeNullableBitmap16(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableBitmap32(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableBitmap64(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableBitmap8(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableBoolean(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableCharString(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)

func subscribeAttributeNullableEnum16(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableEnum8(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableEnumAttr(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableFloatDouble(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableFloatSingle(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt16s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt16u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt24s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt24u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt32s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt32u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt40s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt40u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt48s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt48u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt56s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt56u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt64s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt64u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt8s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableInt8u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableOctetString(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (Data?, (any Error)?) -> Void)

func subscribeAttributeNullableRangeRestrictedInt16s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableRangeRestrictedInt16u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableRangeRestrictedInt8s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableRangeRestrictedInt8u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNullableStruct(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (MTRUnitTestingClusterSimpleStruct?, (any Error)?) -> Void)

func subscribeAttributeOctetString(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (Data?, (any Error)?) -> Void)

func subscribeAttributeRangeRestrictedInt16s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeRangeRestrictedInt16u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeRangeRestrictedInt8s(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeRangeRestrictedInt8u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeStructAttr(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (MTRUnitTestingClusterSimpleStruct?, (any Error)?) -> Void)

func subscribeAttributeTimedWriteBoolean(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeUnsupported(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeVendorId(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeWriteOnlyInt8u(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func test(completion: MTRStatusCompletion)

func test(with: MTRUnitTestingClusterTestParams?, completion: MTRStatusCompletion)

func testAddArguments(with: MTRUnitTestingClusterTestAddArgumentsParams, completion: (MTRUnitTestingClusterTestAddArgumentsResponseParams?, (any Error)?) -> Void)

func testComplexNullableOptionalRequest(with: MTRUnitTestingClusterTestComplexNullableOptionalRequestParams, completion: (MTRUnitTestingClusterTestComplexNullableOptionalResponseParams?, (any Error)?) -> Void)

func testEmitTestEventRequest(with: MTRUnitTestingClusterTestEmitTestEventRequestParams, completion: (MTRUnitTestingClusterTestEmitTestEventResponseParams?, (any Error)?) -> Void)

func testEmitTestFabricScopedEventRequest(with: MTRUnitTestingClusterTestEmitTestFabricScopedEventRequestParams, completion: (MTRUnitTestingClusterTestEmitTestFabricScopedEventResponseParams?, (any Error)?) -> Void)

func testEnumsRequest(with: MTRUnitTestingClusterTestEnumsRequestParams, completion: (MTRUnitTestingClusterTestEnumsResponseParams?, (any Error)?) -> Void)

func testListInt8UArgumentRequest(with: MTRUnitTestingClusterTestListInt8UArgumentRequestParams, completion: (MTRUnitTestingClusterBooleanResponseParams?, (any Error)?) -> Void)

func testListInt8UReverseRequest(with: MTRUnitTestingClusterTestListInt8UReverseRequestParams, completion: (MTRUnitTestingClusterTestListInt8UReverseResponseParams?, (any Error)?) -> Void)

func testListNestedStructListArgumentRequest(with: MTRUnitTestingClusterTestListNestedStructListArgumentRequestParams, completion: (MTRUnitTestingClusterBooleanResponseParams?, (any Error)?) -> Void)

func testListStructArgumentRequest(with: MTRUnitTestingClusterTestListStructArgumentRequestParams, completion: (MTRUnitTestingClusterBooleanResponseParams?, (any Error)?) -> Void)

func testNestedStructArgumentRequest(with: MTRUnitTestingClusterTestNestedStructArgumentRequestParams, completion: (MTRUnitTestingClusterBooleanResponseParams?, (any Error)?) -> Void)

func testNestedStructListArgumentRequest(with: MTRUnitTestingClusterTestNestedStructListArgumentRequestParams, completion: (MTRUnitTestingClusterBooleanResponseParams?, (any Error)?) -> Void)

func testNotHandled(completion: MTRStatusCompletion)

func testNotHandled(with: MTRUnitTestingClusterTestNotHandledParams?, completion: MTRStatusCompletion)

func testNullableOptionalRequest(completion: (MTRUnitTestingClusterTestNullableOptionalResponseParams?, (any Error)?) -> Void)

func testNullableOptionalRequest(with: MTRUnitTestingClusterTestNullableOptionalRequestParams?, completion: (MTRUnitTestingClusterTestNullableOptionalResponseParams?, (any Error)?) -> Void)

func testSimpleArgumentRequest(with: MTRUnitTestingClusterTestSimpleArgumentRequestParams, completion: (MTRUnitTestingClusterTestSimpleArgumentResponseParams?, (any Error)?) -> Void)

func testSimpleOptionalArgumentRequest(completion: MTRStatusCompletion)

func testSimpleOptionalArgumentRequest(with: MTRUnitTestingClusterTestSimpleOptionalArgumentRequestParams?, completion: MTRStatusCompletion)

func testSpecific(completion: (MTRUnitTestingClusterTestSpecificResponseParams?, (any Error)?) -> Void)

func testSpecific(with: MTRUnitTestingClusterTestSpecificParams?, completion: (MTRUnitTestingClusterTestSpecificResponseParams?, (any Error)?) -> Void)

func testStructArgumentRequest(with: MTRUnitTestingClusterTestStructArgumentRequestParams, completion: (MTRUnitTestingClusterBooleanResponseParams?, (any Error)?) -> Void)

func testStructArrayArgumentRequest(with: MTRUnitTestingClusterTestStructArrayArgumentRequestParams, completion: (MTRUnitTestingClusterTestStructArrayArgumentResponseParams?, (any Error)?) -> Void)

func testUnknownCommand(completion: MTRStatusCompletion)

func testUnknownCommand(with: MTRUnitTestingClusterTestUnknownCommandParams?, completion: MTRStatusCompletion)

func timedInvokeRequest(completion: MTRStatusCompletion)

func timedInvokeRequest(with: MTRUnitTestingClusterTimedInvokeRequestParams?, completion: MTRStatusCompletion)

func writeAttributeBitmap16(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeBitmap16(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeBitmap32(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeBitmap32(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeBitmap64(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeBitmap64(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeBitmap8(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeBitmap8(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeBoolean(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeBoolean(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeCharString(withValue: String, completion: MTRStatusCompletion)

func writeAttributeCharString(withValue: String, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeClusterErrorBoolean(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeClusterErrorBoolean(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeEnum16(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeEnum16(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeEnum8(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeEnum8(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeEnumAttr(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeEnumAttr(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeEpochS(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeEpochS(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeEpochUs(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeEpochUs(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeFloatDouble(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeFloatDouble(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeFloatSingle(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeFloatSingle(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeGeneralErrorBoolean(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeGeneralErrorBoolean(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt16s(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt16s(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt16u(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt16u(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt24s(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt24s(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt24u(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt24u(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt32s(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt32s(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt32u(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt32u(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt40s(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt40s(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt40u(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt40u(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt48s(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt48s(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt48u(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt48u(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt56s(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt56s(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt56u(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt56u(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt64s(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt64s(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt64u(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt64u(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt8s(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt8s(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInt8u(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInt8u(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeListFabricScoped(withValue: [Any], completion: MTRStatusCompletion)

func writeAttributeListFabricScoped(withValue: [Any], params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeListInt8u(withValue: [Any], completion: MTRStatusCompletion)

func writeAttributeListInt8u(withValue: [Any], params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeListLongOctetString(withValue: [Any], completion: MTRStatusCompletion)

func writeAttributeListLongOctetString(withValue: [Any], params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeListNullablesAndOptionalsStruct(withValue: [Any], completion: MTRStatusCompletion)

func writeAttributeListNullablesAndOptionalsStruct(withValue: [Any], params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeListOctetString(withValue: [Any], completion: MTRStatusCompletion)

func writeAttributeListOctetString(withValue: [Any], params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeListStructOctetString(withValue: [Any], completion: MTRStatusCompletion)

func writeAttributeListStructOctetString(withValue: [Any], params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeLongCharString(withValue: String, completion: MTRStatusCompletion)

func writeAttributeLongCharString(withValue: String, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeLongOctetString(withValue: Data, completion: MTRStatusCompletion)

func writeAttributeLongOctetString(withValue: Data, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableBitmap16(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableBitmap16(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableBitmap32(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableBitmap32(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableBitmap64(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableBitmap64(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableBitmap8(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableBitmap8(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableBoolean(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableBoolean(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableCharString(withValue: String?, completion: MTRStatusCompletion)

func writeAttributeNullableCharString(withValue: String?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableEnum16(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableEnum16(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableEnum8(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableEnum8(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableEnumAttr(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableEnumAttr(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableFloatDouble(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableFloatDouble(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableFloatSingle(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableFloatSingle(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt16s(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt16s(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt16u(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt16u(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt24s(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt24s(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt24u(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt24u(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt32s(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt32s(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt32u(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt32u(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt40s(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt40s(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt40u(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt40u(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt48s(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt48s(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt48u(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt48u(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt56s(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt56s(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt56u(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt56u(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt64s(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt64s(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt64u(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt64u(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt8s(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt8s(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableInt8u(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableInt8u(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableOctetString(withValue: Data?, completion: MTRStatusCompletion)

func writeAttributeNullableOctetString(withValue: Data?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt16s(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt16s(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt16u(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt16u(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt8s(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt8s(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt8u(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeNullableRangeRestrictedInt8u(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeNullableStruct(withValue: MTRUnitTestingClusterSimpleStruct?, completion: MTRStatusCompletion)

func writeAttributeNullableStruct(withValue: MTRUnitTestingClusterSimpleStruct?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeOctetString(withValue: Data, completion: MTRStatusCompletion)

func writeAttributeOctetString(withValue: Data, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt16s(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt16s(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt16u(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt16u(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt8s(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt8s(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt8u(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeRangeRestrictedInt8u(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeStructAttr(withValue: MTRUnitTestingClusterSimpleStruct, completion: MTRStatusCompletion)

func writeAttributeStructAttr(withValue: MTRUnitTestingClusterSimpleStruct, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeTimedWriteBoolean(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeTimedWriteBoolean(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeUnsupported(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeUnsupported(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeVendorId(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeVendorId(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeWriteOnlyInt8u(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeWriteOnlyInt8u(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

### Type Methods

class func readAttributeAcceptedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAttributeList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeBitmap16(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBitmap32(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBitmap64(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBitmap8(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBoolean(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeCharString(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (String?, (any Error)?) -> Void)

class func readAttributeClusterErrorBoolean(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEnum16(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEnum8(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEnumAttr(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEpochS(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEpochUs(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFloatDouble(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFloatSingle(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneralErrorBoolean(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeInt16s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt16u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt24s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt24u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt32s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt32u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt40s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt40u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt48s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt48u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt56s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt56u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt64s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt64u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt8s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeInt8u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeListFabricScoped(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeListInt8u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeListLongOctetString(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeListNullablesAndOptionalsStruct(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeListOctetString(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeListStructOctetString(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeLongCharString(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (String?, (any Error)?) -> Void)

class func readAttributeLongOctetString(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (Data?, (any Error)?) -> Void)

class func readAttributeNullableBitmap16(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableBitmap32(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableBitmap64(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableBitmap8(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableBoolean(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableCharString(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (String?, (any Error)?) -> Void)

class func readAttributeNullableEnum16(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableEnum8(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableEnumAttr(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableFloatDouble(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableFloatSingle(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt16s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt16u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt24s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt24u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt32s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt32u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt40s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt40u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt48s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt48u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt56s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt56u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt64s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt64u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt8s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableInt8u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableOctetString(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (Data?, (any Error)?) -> Void)

class func readAttributeNullableRangeRestrictedInt16s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableRangeRestrictedInt16u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableRangeRestrictedInt8s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableRangeRestrictedInt8u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNullableStruct(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (MTRUnitTestingClusterSimpleStruct?, (any Error)?) -> Void)

class func readAttributeOctetString(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (Data?, (any Error)?) -> Void)

class func readAttributeRangeRestrictedInt16s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeRangeRestrictedInt16u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeRangeRestrictedInt8s(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeRangeRestrictedInt8u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeStructAttr(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (MTRUnitTestingClusterSimpleStruct?, (any Error)?) -> Void)

class func readAttributeTimedWriteBoolean(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeUnsupported(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeVendorId(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeWriteOnlyInt8u(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

## Relationships

### Inherits From

- MTRGenericBaseCluster

### Inherited By

- MTRBaseClusterTestCluster

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

