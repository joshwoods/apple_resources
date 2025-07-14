

- Matter
-  MTRClusterTestCluster Deprecated

Class

# MTRClusterTestCluster

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
class MTRClusterTestCluster
```

Deprecated

Please use MTRClusterUnitTesting

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)

### Instance Methods

func simpleStructEchoRequest(with: MTRTestClusterClusterSimpleStructEchoRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterSimpleStructResponseParams?, (any Error)?) -> Void)

func test(with: MTRTestClusterClusterTestParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func test(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func testAddArguments(with: MTRTestClusterClusterTestAddArgumentsParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterTestAddArgumentsResponseParams?, (any Error)?) -> Void)

func testComplexNullableOptionalRequest(with: MTRTestClusterClusterTestComplexNullableOptionalRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterTestComplexNullableOptionalResponseParams?, (any Error)?) -> Void)

func testEmitTestEventRequest(with: MTRTestClusterClusterTestEmitTestEventRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterTestEmitTestEventResponseParams?, (any Error)?) -> Void)

func testEmitTestFabricScopedEventRequest(with: MTRTestClusterClusterTestEmitTestFabricScopedEventRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterTestEmitTestFabricScopedEventResponseParams?, (any Error)?) -> Void)

func testEnumsRequest(with: MTRTestClusterClusterTestEnumsRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterTestEnumsResponseParams?, (any Error)?) -> Void)

func testListInt8UArgumentRequest(with: MTRTestClusterClusterTestListInt8UArgumentRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterBooleanResponseParams?, (any Error)?) -> Void)

func testListInt8UReverseRequest(with: MTRTestClusterClusterTestListInt8UReverseRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterTestListInt8UReverseResponseParams?, (any Error)?) -> Void)

func testListNestedStructListArgumentRequest(with: MTRTestClusterClusterTestListNestedStructListArgumentRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterBooleanResponseParams?, (any Error)?) -> Void)

func testListStructArgumentRequest(with: MTRTestClusterClusterTestListStructArgumentRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterBooleanResponseParams?, (any Error)?) -> Void)

func testNestedStructArgumentRequest(with: MTRTestClusterClusterTestNestedStructArgumentRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterBooleanResponseParams?, (any Error)?) -> Void)

func testNestedStructListArgumentRequest(with: MTRTestClusterClusterTestNestedStructListArgumentRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterBooleanResponseParams?, (any Error)?) -> Void)

func testNotHandled(with: MTRTestClusterClusterTestNotHandledParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func testNotHandled(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func testNullableOptionalRequest(with: MTRTestClusterClusterTestNullableOptionalRequestParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterTestNullableOptionalResponseParams?, (any Error)?) -> Void)

func testNullableOptionalRequest(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterTestNullableOptionalResponseParams?, (any Error)?) -> Void)

func testSimpleArgumentRequest(with: MTRTestClusterClusterTestSimpleArgumentRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterTestSimpleArgumentResponseParams?, (any Error)?) -> Void)

func testSimpleOptionalArgumentRequest(with: MTRTestClusterClusterTestSimpleOptionalArgumentRequestParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func testSimpleOptionalArgumentRequest(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func testSpecific(with: MTRTestClusterClusterTestSpecificParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterTestSpecificResponseParams?, (any Error)?) -> Void)

func testSpecific(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterTestSpecificResponseParams?, (any Error)?) -> Void)

func testStructArgumentRequest(with: MTRTestClusterClusterTestStructArgumentRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterBooleanResponseParams?, (any Error)?) -> Void)

func testStructArrayArgumentRequest(with: MTRTestClusterClusterTestStructArrayArgumentRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRTestClusterClusterTestStructArrayArgumentResponseParams?, (any Error)?) -> Void)

func testUnknownCommand(with: MTRTestClusterClusterTestUnknownCommandParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func testUnknownCommand(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func timedInvokeRequest(with: MTRTestClusterClusterTimedInvokeRequestParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func timedInvokeRequest(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

## Relationships

### Inherits From

- MTRClusterUnitTesting

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

