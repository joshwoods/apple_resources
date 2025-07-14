

- PHASE
- PHASEGroup
-  register(engine:) 

Instance Method

# register(engine:)

Adds the group to the engine’s dictionary.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func register(engine: PHASEEngine)
```

## Parameters 

`engine`  

The engine with which to register this group.

## Discussion

The function generates an exception if the argument is `nil` or if engine already contains the group. For more information, see groups.

## See Also

### Defining the Group

func unregisterFromEngine()

Removes the group from the engine’s dictionary.

