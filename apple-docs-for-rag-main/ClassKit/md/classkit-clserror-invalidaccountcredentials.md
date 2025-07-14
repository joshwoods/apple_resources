

- ClassKit
- CLSError
-  invalidAccountCredentials 

Type Property

# invalidAccountCredentials

iOS 15.1+iPadOS 15.1+Mac Catalyst 15.1+macOS 12.0+visionOS 1.0+

``` source
static var invalidAccountCredentials: CLSError.Code { get }
```

## See Also

### Error Codes

static var none: CLSError.Code

No error.

static var authorizationDenied: CLSError.Code

The app isn’t authorized to perform the requested operation.

static var classKitUnavailable: CLSError.Code

ClassKit isn’t available on this device.

static var databaseInaccessible: CLSError.Code

ClassKit isn’t accessible because the device is locked.

static var invalidArgument: CLSError.Code

An invalid argument was provided to the API.

static var invalidCreate: CLSError.Code

An attempt to save a new object that already exists in the data store failed.

static var invalidModification: CLSError.Code

An attempt to modify a read-only object failed.

static var invalidUpdate: CLSError.Code

ClassKit failed to save an updated object in the data store.

static var limits: CLSError.Code

A limit has been exceeded.

static var partialFailure: CLSError.Code

ClassKit encountered more than one error.

enum Code

Error codes that ClassKit issues.

