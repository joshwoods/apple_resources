

- Model I/O
- MDLMaterialProperty
-  setProperties(\_:) 

Instance Method

# setProperties(\_:)

Sets the material property’s attributes to those of the specified material property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func setProperties(_ property: MDLMaterialProperty)
```

## Parameters 

`property`  

The material property from which to copy data.

## Discussion

Use this method to copy data from one MDLMaterialProperty instance to another—for example, to make one material property of a MDLScatteringFunction object match the value of another.

