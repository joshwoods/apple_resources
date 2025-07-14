

- Automator
- AMError
- AMError.Code
-  AMError.Code.workflowPropertyListInvalidError 

Case

# AMError.Code.workflowPropertyListInvalidError

An error that indicates an attempt to open a workflow document whose property list couldn’t be read.

Mac Catalyst 14.0+macOS 10.4+

``` source
case workflowPropertyListInvalidError
```

## Discussion

The property list document (`document.wflow`) could be missing, damaged, or constructed improperly.

## See Also

### Workflow Errors

case workflowActionsNotLoadedError

An error that indicates one of the actions of the workflow couldn’t be loaded.

case workflowNewerActionVersionError

An error that indicates an action in a workflow is newer than the installed action.

case workflowNewerVersionError

An error that indicates an attempt to open a workflow document that was saved with a newer version of Automator.

case workflowNoEnabledActionsError

An error that indicates there are no enabled actions in the workflow.

case workflowOlderActionVersionError

An error that indicates an action in a workflow is older than the installed action.

