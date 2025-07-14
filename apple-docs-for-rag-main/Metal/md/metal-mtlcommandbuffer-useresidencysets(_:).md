

- Metal
- MTLCommandBuffer
-  useResidencySets(\_:) 

Instance Method

# useResidencySets(\_:)

Attaches multiple residency sets to the command buffer.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS

``` source
func useResidencySets(_ residencySets: [any MTLResidencySet])
```

## Parameters 

`residencySets`  

An array of residency sets, each of which contains resource allocations, such as MTLBuffer, MTLTexture, and MTLHeap instances.

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

## Discussion

See Simplifying GPU Resource Management with Residency Sets and MTLResidencySet for more information.

## See Also

### Attaching Residency Sets

func useResidencySet(any MTLResidencySet)

Attaches a residency set to the command buffer.

**Required**

