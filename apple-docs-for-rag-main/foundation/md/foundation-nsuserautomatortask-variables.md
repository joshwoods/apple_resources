

- Foundation
- NSUserAutomatorTask
-  variables 

Instance Property

# variables

The variables required by the Automator workflow.

macOS 10.8+

``` source
var variables: [String : Any]? { get set }
```

## See Also

### Executing Automator Tasks

func execute(withInput: (any NSSecureCoding)?, completionHandler: NSUserAutomatorTask.CompletionHandler?)

Execute the Automator workflow by providing it as securely coded input.

