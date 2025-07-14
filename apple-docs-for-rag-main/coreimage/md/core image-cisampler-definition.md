

- Core Image
- CISampler
-  definition 

Instance Property

# definition

The domain of definition (DOD) of the sampler

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
var definition: CIFilterShape { get }
```

## Discussion

The DOD contains all nontransparent pixels produced by referencing the sampler.

## See Also

### Getting Information About the Sampler Object

var extent: CGRect

The rectangle that specifies the extent of the sampler

