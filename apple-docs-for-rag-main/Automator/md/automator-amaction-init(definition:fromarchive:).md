

- Automator
- AMAction
-  init(definition:fromArchive:) 

Initializer

# init(definition:fromArchive:)

Initializes the action with the specified definition.

Mac Catalyst 14.0+macOS 10.4+

``` source
init?(
    definition dict: [String : Any]?,
    fromArchive archived: Bool
)
```

## Parameters 

`dict`  

A dictionary that describes the action, including any custom definition properties.

`archived`  

If the action is being unarchived, true; otherwise, false.

## Return Value

The initialized action.

## Discussion

This is the primary initializer for all Automator classes. The Automator app sends this message to instances of AMAction both when it loads actions bundles and when it unarchives them.

The AMAction object being instantiated should perform whatever initializations are necessary after invoking `super`’s implementation of this method. It can then examine the values in `dict`, particularly if the action had been archived with custom definition properties.

## See Also

### Initializing and Encoding

init(contentsOf: URL) throws

Loads an Automator action from a file URL.

func write(to: NSMutableDictionary)

Examines the parameters and other configuration information specified in the passed dictionary and adds its own information to it if appropriate.

