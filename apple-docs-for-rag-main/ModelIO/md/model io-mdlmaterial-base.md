

- Model I/O
- MDLMaterial
-  base 

Instance Property

# base

Another material object from which this material’s properties are derived.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var base: MDLMaterial? { get set }
```

## Discussion

When you use the property(with:), propertyNamed(_:), or subscript(_:) method to access material properties, the MDLMaterial class first checks whether the material itself has a material property with the specified name or semantic. If not, those methods forward to the corresponding method of the other MDLMaterial object specified by this property.

Use this method to create sets of materials that share most of their material properties but differ in others. For example, you can have a set of objects in the same scene with the same general style of surface appearance (determined by the scatteringFunction property) but with different values for the baseColor material property.

