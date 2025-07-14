

- Metal
- MTLCommandBuffer
-  useResidencySet(\_:) 

Instance Method

# useResidencySet(\_:)

Attaches a residency set to the command buffer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func useResidencySet(_ residencySet: any MTLResidencySet)
```

**Required**

## Parameters 

`residencySet`  

A residency set that contains resource allocations, such as MTLBuffer, MTLTexture, and MTLHeap instances.

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

## Discussion

See Simplifying GPU Resource Management with Residency Sets and MTLResidencySet for more information.

## See Also

### Attaching Residency Sets

func useResidencySets([any MTLResidencySet])

Attaches multiple residency sets to the command buffer.

