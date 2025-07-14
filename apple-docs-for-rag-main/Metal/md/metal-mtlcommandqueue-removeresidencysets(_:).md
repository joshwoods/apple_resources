

- Metal
- MTLCommandQueue
-  removeResidencySets(\_:) 

Instance Method

# removeResidencySets(\_:)

Detaches multiple residency sets from the command queue, which prevents Metal from attaching them to the queue’s command buffers as you commit them.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS

``` source
func removeResidencySets(_ residencySets: [any MTLResidencySet])
```

## Parameters 

`residencySets`  

An array of residency sets, each of which contains resource allocations, such as MTLBuffer, MTLTexture, and MTLHeap instances.

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

## Discussion

The method doesn’t remove the residency sets from command buffers the queue owns with a status property that’s equal to MTLCommandBufferStatus.committed or MTLCommandBufferStatus.scheduled.

See Simplifying GPU Resource Management with Residency Sets and MTLResidencySet for more information.

## See Also

### Detaching Residency Sets

func removeResidencySet(any MTLResidencySet)

Detaches a residency set from the command queue, which prevents Metal from attaching it to the queue’s command buffers as you commit them.

**Required**

