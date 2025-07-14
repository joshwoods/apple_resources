

- Matter
-  MTRDeviceController 

Class

# MTRDeviceController

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRDeviceController
```

## Mentioned in 

Onboarding a Matter device

## Topics

### Initializers

init(parameters: MTRDeviceControllerAbstractParameters) throws

### Instance Properties

var controllerNodeID: NSNumber?

var controllerNodeId: NSNumber?Deprecated

var isRunning: Bool

var uniqueIdentifier: UUID

var devices: [MTRDevice]

Returns the list of MTRDevice instances that this controller has loaded into memory. Returns an empty array if no devices are in memory.

var isSuspended: Bool

If true, the controller has been suspended via `suspend` and not resumed yet.

var nodesWithStoredData: [NSNumber]

Returns the list of node IDs for which this controller has stored information. Returns empty list if the controller does not have any information stored.

### Instance Methods

func add(MTRServerEndpoint) -> Bool

func attestationChallenge(forDeviceID: NSNumber) -> Data?

func cancelCommissioning(forNodeID: NSNumber) throws

func commissionDevice(UInt64, commissioningParams: MTRCommissioningParameters) throwsDeprecated

func commissionNode(withID: NSNumber, commissioningParams: MTRCommissioningParameters) throws

func computePaseVerifier(UInt32, iterations: UInt32, salt: Data) -> Data?Deprecated

func continueCommissioningDevice(UnsafeMutableRawPointer, ignoreAttestationFailure: Bool) throws

func deviceBeingCommissioned(withNodeID: NSNumber) throws -> MTRBaseDevice

func fetchAttestationChallenge(forDeviceId: UInt64) -> Data?Deprecated

func getBaseDevice(UInt64, queue: dispatch_queue_t, completionHandler: MTRDeviceConnectionCallback) -> BoolDeprecated

func getDeviceBeingCommissioned(UInt64) throws -> MTRBaseDeviceDeprecated

func openPairingWindow(UInt64, duration: Int) throwsDeprecated

func openPairingWindow(withPIN: UInt64, duration: Int, discriminator: Int, setupPIN: Int) throws -> StringDeprecated

func pairDevice(UInt64, address: String, port: UInt16, setupPINCode: UInt32) throwsDeprecated

func pairDevice(UInt64, discriminator: UInt16, setupPINCode: UInt32) throwsDeprecated

func pairDevice(UInt64, onboardingPayload: String) throwsDeprecated

func preWarmCommissioningSession()Deprecated

func remove(MTRServerEndpoint, queue: dispatch_queue_t, completion: () -> Void)

func setDeviceControllerDelegate(any MTRDeviceControllerDelegate, queue: dispatch_queue_t)

func setNocChainIssuer(any MTRNOCChainIssuer, queue: dispatch_queue_t)Deprecated

func setPairingDelegate(any MTRDevicePairingDelegate, queue: dispatch_queue_t)Deprecated

func setupCommissioningSession(with: MTRSetupPayload, newNodeID: NSNumber) throws

func setupCommissioningSession(withDiscoveredDevice: MTRCommissionableBrowserResult, payload: MTRSetupPayload, newNodeID: NSNumber) throws

func shutdown()

func startBrowse(forCommissionables: any MTRCommissionableBrowserDelegate, queue: dispatch_queue_t) -> Bool

func stopBrowseForCommissionables() -> Bool

func stopDevicePairing(UInt64) throwsDeprecated

func add(any MTRDeviceControllerDelegate, queue: dispatch_queue_t)

Adds a Delegate to the device controller as well as the Queue on which the Delegate callbacks will be triggered

func forgetDevice(withNodeID: NSNumber)

Forget any information we have about the device with the given node ID. That includes clearing any information we have stored about it.

func remove(MTRServerEndpoint)

Remove the given server endpoint without being notified when the removal completes.

func remove(any MTRDeviceControllerDelegate)

Removes a Delegate from the device controller

func resume()

Resume the controller. This has no effect if the controller is not suspended.

func suspend()

Suspend the controller. This will attempt to stop all network traffic associated with the controller. The controller will remain suspended until it is resumed.

### Type Methods

class func computePASEVerifier(forSetupPasscode: NSNumber, iterations: NSNumber, salt: Data) throws -> Data

class func decodeXPCReadParams([String : Any]?) -> MTRReadParams?

class func decodeXPCResponseValues([[String : Any]]?) -> [[String : Any]]?

class func decodeXPCSubscribeParams([String : Any]?) -> MTRSubscribeParams?

class func encodeXPCReadParams(MTRReadParams) -> [String : Any]?

class func encodeXPCResponseValues([[String : Any]]?) -> [[String : Any]]?

class func encodeXPCSubscribeParams(MTRSubscribeParams?) -> [String : Any]?

class func sharedController(withID: (any NSCopying)?, xpcConnect: MTRXPCConnectBlock) -> MTRDeviceController

class func sharedController(withId: (any NSCopying)?, xpcConnect: MTRXPCConnectBlock) -> MTRDeviceControllerDeprecated

class func xpcInterfaceForClientProtocol() -> NSXPCInterface

class func xpcInterfaceForServerProtocol() -> NSXPCInterface

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

