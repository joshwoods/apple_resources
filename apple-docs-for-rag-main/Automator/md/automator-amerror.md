

- Automator
-  AMError 

Structure

# AMError

An Automator error.

Mac Catalyst 14.0+macOS 10.4+

``` source
struct AMError
```

## Topics

### Error Codes

static var workflowActionsNotLoadedError: AMError.Code

An error that indicates one of the actions of the workflow couldn’t be loaded.

static var workflowNewerActionVersionError: AMError.Code

An error that indicates an action in a workflow is newer than the installed action.

static var workflowNewerVersionError: AMError.Code

An error that indicates an attempt to open a workflow document that was saved with a newer version of Automator.

static var workflowNoEnabledActionsError: AMError.Code

An error that indicates there are no enabled actions in the workflow.

static var workflowOlderActionVersionError: AMError.Code

An error that indicates an action in a workflow is older than the installed action.

static var workflowPropertyListInvalidError: AMError.Code

An error that indicates an attempt to open a workflow document whose property list couldn’t be read.

static var userCanceledError: AMError.Code

An error that indicates the user cancelled.

static var actionApplicationResourceError: AMError.Code

An error that indicates an app required by the action is not found.

static var actionApplicationVersionResourceError: AMError.Code

An error that indicates an app required by the action is the wrong version.

static var actionArchitectureMismatchError: AMError.Code

An error that indicates the action’s binary is not compatible with the current processor.

static var actionExceptionError: AMError.Code

An error that indicates an action encounters an exception while running.

static var actionExecutionError: AMError.Code

An error that indicates an action encounters an error while running (reason unknown).

static var actionFailedGatekeeperError: AMError.Code

An error that indicates the action doesn’t meet the Gatekeeper security policy.

static var actionFileResourceError: AMError.Code

An error that indicates a file required by the action is not found.

static var actionInitializationError: AMError.Code

An error that indicates Automator is unable to initialize an action (reason unknown).

static var actionInsufficientDataError: AMError.Code

An error that indicates the action requires input data to run, but none was supplied.

static var actionIsDeprecatedError: AMError.Code

An error that indicates the action has been deprecated.

static var actionLicenseResourceError: AMError.Code

An error that indicates a license required by the action was not found.

static var actionLinkError: AMError.Code

An error that indicates the action’s executable failed to load due to linking issues.

static var actionLoadError: AMError.Code

An error that indicates the action’s executable failed to load.

static var actionMalwareError: AMError.Code

An error that indicates the action has been identified as malware by XProtect.

static var actionNotLoadableError: AMError.Code

An error that indicates the action’s executable is of a type that is not loadable in the current process.

static var actionPropertyListInvalidError: AMError.Code

An error that indicates the property list for an action is invalid.

static var actionQuarantineError: AMError.Code

An error that indicates action has been quarantined by XProtect, the antimalware system on the Mac.

static var actionRequiredActionResourceError: AMError.Code

An error that indicates an action required by the action is not loaded.

static var actionRuntimeMismatchError: AMError.Code

An error that indicates an attempt was made to load an action that is not compiled in a way that is compatible with the current app.

static var actionSignatureCorruptError: AMError.Code

An error that indicates developer signature for this action is corrupted.

static var actionThirdPartyActionsNotAllowedError: AMError.Code

An error that indicates the action is a third party action, and loading it has not been allowed by the user.

static var actionXPCError: AMError.Code

An error that indicates the remote process running the action has crashed.

static var actionXProtectError: AMError.Code

An error that indicates XProtect is unable to successfully analyze the action.

static var noSuchActionError: AMError.Code

An error that indicates the action could not be located on the system.

static var conversionFailedError: AMError.Code

An error that occurs when, for example, the converter encounters an error converting data from one type to another.

static var conversionNoDataError: AMError.Code

An error that occurs when the converter determines that the conversion, though possible, would produce a nil result.

static var conversionNotPossibleError: AMError.Code

An error that occurs when the converter determines that it is unable to convert from one data type to another.

enum Code

Automator error codes.

### Error Domain

var AMAutomatorErrorDomain: String

A string that identifies the Automator error domain.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

var AMAutomatorErrorDomain: String

A string that identifies the Automator error domain.

var AMActionErrorKey: String

A key to retrieve the action that caused an error.

enum Code

Automator error codes.

