

- Foundation
- NSScriptCommandDescription
-  createCommandInstance(with:) 

Instance Method

# createCommandInstance(with:)

Creates and returns an instance of the command object described by the receiver in the specified memory zone.

Mac Catalyst 13.0+macOS 10.0+

``` source
func createCommandInstance(with zone: NSZone? = nil) -> NSScriptCommand
```

## Parameters 

`zone`  

The memory zone from which to allocate the command.

## Return Value

The command object, instantiated from NSScriptCommand or a subclass.

## See Also

### Creating Commands

func createCommandInstance() -> NSScriptCommand

Creates and returns an instance of the command object described by the receiver.

