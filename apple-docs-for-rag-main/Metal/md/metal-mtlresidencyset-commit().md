

- Metal
- MTLResidencySet
-  commit() 

Instance Method

# commit()

Applies any pending additions to and removals from the residency set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func commit()
```

**Required**

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

## Discussion

Call the method when have no other changes to stage, such as with addAllocation(_:), removeAllocation(_:), and their sibling methods.

