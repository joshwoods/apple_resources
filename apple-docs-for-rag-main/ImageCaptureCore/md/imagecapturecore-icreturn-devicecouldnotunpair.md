

- ImageCaptureCore
- ICReturn
-  deviceCouldNotUnpair 

Type Property

# deviceCouldNotUnpair

An unpairing request for an Apple Device failed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.9+visionOS 1.0+Xcode 11.0+

``` source
static var deviceCouldNotUnpair: ICReturn.Code { get }
```

## See Also

### Error Codes

static var communicationTimedOut: ICReturn.Code

Communication between different components of Image Capture timed out.

static var deleteFilesCanceled: ICReturn.Code

A request to delete files was canceled.

static var deleteFilesFailed: ICReturn.Code

A request to delete files failed.

static var deviceCommandGeneralFailure: ICReturn.Code

The device has experienced a general failure.

static var deviceCouldNotPair: ICReturn.Code

A pairing request for an Apple Device failed.

static var deviceFailedToCloseSession: ICReturn.Code

Failed to close a session on a specified device.

static var deviceFailedToCompleteTransfer: ICReturn.Code

Failed to complete a data transaction.

static var deviceFailedToOpenSession: ICReturn.Code

Failed to open a session on a specified device.

static var deviceFailedToSendData: ICReturn.Code

Failed to send data.

static var deviceFailedToTakePicture: ICReturn.Code

Failed to take a tethered-capture picture on a camera device.

static var deviceIsBusyEnumerating: ICReturn.Code

The device is currently enumerating assets.

static var deviceIsPasscodeLocked: ICReturn.Code

The device is locked with a passcode. Its contents cannot be seen unless it is unlocked.

static var deviceNeedsCredentials: ICReturn.Code

The device reports credentials are required to open the device.

static var deviceSoftwareInstallationCanceled: ICReturn.Code

Software installation for the device has been canceled.

static var deviceSoftwareInstallationCompleted: ICReturn.Code

Software installation for the device has completed successfully.

static var deviceSoftwareInstallationFailed: ICReturn.Code

Software installation for the device failed.

static var deviceSoftwareIsBeingInstalled: ICReturn.Code

Failed to open session because software to communicate with the device is being installed.

static var deviceSoftwareNotAvailable: ICReturn.Code

Software for the device is not available from Apple.

static var deviceSoftwareNotInstalled: ICReturn.Code

Failed to open session because software to communicate with the device is not installed.

static var downloadCanceled: ICReturn.Code

A download operation was canceled.

static var downloadFailed: ICReturn.Code

A non-specific error occurred while downloading a file.

static var exFATVolumeInvalid: ICReturn.Code

EXFAT volume is invalid, and cannot be enumerated.

static var failedToCompletePassThroughCommand: ICReturn.Code

Failed to complete a pass-through (e.g., PTP pass-through) command.

static var failedToCompleteSendMessageRequest: ICReturn.Code

A request to send a message to a device failed.

static var failedToDisabeTethering: ICReturn.Code

A request to send a message to a device failed.

static var failedToEnabeTethering: ICReturn.Code

Failed to enable tethered-capture on a camera device.

static var invalidParam: ICReturn.Code

An invalid parameter was found.

static var multiErrorDictionary: ICReturn.Code

Multierror

static var receivedUnsolicitedScannerErrorInfo: ICReturn.Code

An unsolicited error information was received from a scanner.

static var receivedUnsolicitedScannerStatusInfo: ICReturn.Code

An unsolicited status information was received from a scanner.

static var scanOperationCanceled: ICReturn.Code

The scan operation is canceled.

static var scannerFailedToCompleteOverviewScan: ICReturn.Code

Overview scan operation failed to complete on the specified scanner.

static var scannerFailedToCompleteScan: ICReturn.Code

Scan operation failed to complete on the specified scanner.

static var scannerFailedToSelectFunctionalUnit: ICReturn.Code

Failed to select a functional unit on the specified scanner.

static var scannerInUseByLocalUser: ICReturn.Code

Scanner is being used by a local user.

static var scannerInUseByRemoteUser: ICReturn.Code

Scanner is being used by a remote user.

static var sessionNotOpened: ICReturn.Code

Session is not open.

static var success: ICReturn.Code

Operation successful.

static var uploadFailed: ICReturn.Code

A non-specific error occurred while updownloading a file.

enum ICReturn.Code

enum ICReturnCodeOffset

