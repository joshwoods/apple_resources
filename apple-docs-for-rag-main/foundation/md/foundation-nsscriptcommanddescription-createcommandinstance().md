

- Foundation
- NSScriptCommandDescription
-  createCommandInstance() 

Instance Method

# createCommandInstance()

Creates and returns an instance of the command object described by the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func createCommandInstance() -> NSScriptCommand
```

## Return Value

The command object, instantiated from NSScriptCommand or a subclass.

## See Also

### Creating Commands

func createCommandInstance(with: NSZone?) -> NSScriptCommand

Creates and returns an instance of the command object described by the receiver in the specified memory zone.

