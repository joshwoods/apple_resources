

- Automator
- AMWorkflow
-  actions 

Instance Property

# actions

An array of the workflow’s actions.

Mac Catalyst 14.0+macOS 10.4+

``` source
var actions: [AMAction] { get }
```

## Return Value

An array of actions for the workflow file. Actions are instances of classes such as AMBundleAction, AMAppleScriptAction, and AMShellScriptAction.

## See Also

### Getting Information About a Workflow

var fileURL: URL?

A URL that specifies the location of the workflow file.

func valueForVariable(withName: String) -> Any?

Returns the value of the workflow variable with the specified name.

