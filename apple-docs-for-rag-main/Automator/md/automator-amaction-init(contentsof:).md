

- Automator
- AMAction
-  init(contentsOf:) 

Initializer

# init(contentsOf:)

Loads an Automator action from a file URL.

Mac Catalyst 14.0+macOS 10.5+

``` source
init(contentsOf fileURL: URL) throws
```

## Parameters 

`fileURL`  

URL that specifies the location of an action file.

## Return Value

The initialized action.

## Discussion

This method is typically invoked by app that use the AMWorkflow class to embed Automator workflows. It is used to allow creation of actions for a workflow.

## See Also

### Initializing and Encoding

init?(definition: [String : Any]?, fromArchive: Bool)

Initializes the action with the specified definition.

func write(to: NSMutableDictionary)

Examines the parameters and other configuration information specified in the passed dictionary and adds its own information to it if appropriate.

