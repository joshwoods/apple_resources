

- Metal
- MTLDevice
-  makeResidencySet(descriptor:) 

Instance Method

# makeResidencySet(descriptor:)

Creates a residency set, which can move resources in and out of memory residency.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func makeResidencySet(descriptor desc: MTLResidencySetDescriptor) throws -> any MTLResidencySet
```

**Required**

## Parameters 

`desc`  

A descriptor instance that configures the residency set the method creates.

## Return Value

A new MTLResidencySet instance if the method completes successfully; otherwise Swift throws an error and Objective-C returns `nil`.

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

## Discussion

Create an MTLResidencySet by creating and configuring an MTLResidencySetDescriptor instance and pass it to this method.

See Simplifying GPU Resource Management with Residency Sets for more information.

