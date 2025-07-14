

- Audio Toolbox
- AUParameterTree
-  parameter(withAddress:) 

Instance Method

# parameter(withAddress:)

Searches the tree for a parameter with a specific address.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func parameter(withAddress address: AUParameterAddress) -> AUParameter?
```

## Parameters 

`address`  

The address with which to search the tree.

## Return Value

The parameter corresponding to the supplied address, or `nil` if no such parameter exists.

## See Also

### Obtaining Tree Parameters

func parameter(withID: AudioUnitParameterID, scope: AudioUnitScope, element: AudioUnitElement) -> AUParameter?

Searches the tree for a specific version 2 audio unit parameter.

