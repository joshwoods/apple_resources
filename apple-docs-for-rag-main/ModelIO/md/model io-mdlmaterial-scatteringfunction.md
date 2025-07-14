

- Model I/O
- MDLMaterial
-  scatteringFunction 

Instance Property

# scatteringFunction

The collection of material properties that define the material’s response to light.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var scatteringFunction: MDLScatteringFunction { get }
```

## Discussion

A MDLScatteringFunction object defines a Bidirectional Reflectance Distribution Function (BRDF), which determines how a material interacts with lighting to produce a surface appearance. Though you can access the individual material properties in a scattering function directly, a scattering function object lets you work with the collection of lighting-related material properties as a single unit. Use the MDLScatteringFunction class itself to describe a classical Lambertian/Blinn-Phong shading model, or the MDLPhysicallyPlausibleScatteringFunction class to describe a shading model based more closely on real-world physics.

A scattering function determines lighting-related aspects of a material’s appearance, but not all aspects. For features such as opacity and surface deformation, use the methods listed in Working with individual material properties to access the corresponding material properties.

