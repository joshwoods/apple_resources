

- Automator
- AMError
-  actionInsufficientDataError 

Type Property

# actionInsufficientDataError

An error that indicates the action requires input data to run, but none was supplied.

Mac Catalyst 14.0+macOS 10.4+

``` source
static var actionInsufficientDataError: AMError.Code { get }
```

## See Also

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

