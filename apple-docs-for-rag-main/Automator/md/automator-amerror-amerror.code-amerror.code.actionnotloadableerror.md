

- Automator
- AMError
- AMError.Code
-  AMError.Code.actionNotLoadableError 

Case

# AMError.Code.actionNotLoadableError

An error that indicates the action’s executable is of a type that is not loadable in the current process.

Mac Catalyst 14.0+macOS 10.4+

``` source
case actionNotLoadableError
```

## Discussion

If the action uses a custom subclass of AMBundleAction or AMAppleScriptAction, then the most likely problem is that the bundle’s executable is missing or the `NSPrincipleClass` is not set in the `Info.plist`. Users are likely to be confused by a “missing bundle” error, so Automator presents it as the more generic “action not loadable” error.

## See Also

### Action Errors

case actionApplicationResourceError

An error that indicates an app required by the action is not found.

case actionApplicationVersionResourceError

An error that indicates an app required by the action is the wrong version.

case actionArchitectureMismatchError

An error that indicates the action’s binary is not compatible with the current processor.

case actionExceptionError

An error that indicates an action encounters an exception while running.

case actionExecutionError

An error that indicates an action encounters an error while running (reason unknown).

case actionFailedGatekeeperError

An error that indicates the action doesn’t meet the Gatekeeper security policy.

case actionFileResourceError

An error that indicates a file required by the action is not found.

case actionInitializationError

An error that indicates Automator is unable to initialize an action (reason unknown).

case actionInsufficientDataError

An error that indicates the action requires input data to run, but none was supplied.

case actionIsDeprecatedError

An error that indicates the action has been deprecated.

case actionLicenseResourceError

An error that indicates a license required by the action was not found.

case actionLinkError

An error that indicates the action’s executable failed to load due to linking issues.

case actionLoadError

An error that indicates the action’s executable failed to load.

case actionMalwareError

An error that indicates the action has been identified as malware by XProtect.

case actionPropertyListInvalidError

An error that indicates the property list for an action is invalid.

