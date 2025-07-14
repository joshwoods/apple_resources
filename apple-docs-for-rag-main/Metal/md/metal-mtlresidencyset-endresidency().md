

- Metal
- MTLResidencySet
-  endResidency() 

Instance Method

# endResidency()

Informs Metal that the residency set’s allocations no longer need to be resident, and that it can reuse the memory for other allocations.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func endResidency()
```

**Required**

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

