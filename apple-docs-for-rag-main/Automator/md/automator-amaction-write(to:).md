

- Automator
- AMAction
-  write(to:) 

Instance Method

# write(to:)

Examines the parameters and other configuration information specified in the passed dictionary and adds its own information to it if appropriate.

Mac Catalyst 14.0+macOS 10.4+

``` source
func write(to dictionary: NSMutableDictionary)
```

## Parameters 

`dictionary`  

A dictionary that contains parameter and other configuration information about the action.

## Discussion

Automator sends this message to an action object prior to archiving it. In its implementation of this method, the action object should first invoke the superclass implementation.

## See Also

### Initializing and Encoding

init?(definition: [String : Any]?, fromArchive: Bool)

Initializes the action with the specified definition.

init(contentsOf: URL) throws

Loads an Automator action from a file URL.

