

- Metal
- MTLCommandQueue
-  removeResidencySet(\_:) 

Instance Method

# removeResidencySet(\_:)

Detaches a residency set from the command queue, which prevents Metal from attaching it to the queue’s command buffers as you commit them.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func removeResidencySet(_ residencySet: any MTLResidencySet)
```

**Required**

## Parameters 

`residencySet`  

A residency set that contains resource allocations, such as MTLBuffer, MTLTexture, and MTLHeap instances.

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

## Discussion

The method doesn’t remove the residency set from command buffers the queue owns with a status property that’s equal to MTLCommandBufferStatus.committed or MTLCommandBufferStatus.scheduled.

See Simplifying GPU Resource Management with Residency Sets and MTLResidencySet for more information.

## See Also

### Detaching Residency Sets

func removeResidencySets([any MTLResidencySet])

Detaches multiple residency sets from the command queue, which prevents Metal from attaching them to the queue’s command buffers as you commit them.

