

- Metal
- MTLDispatchThreadgroupsIndirectArguments
-  init(threadgroupsPerGrid:) 

Initializer

# init(threadgroupsPerGrid:)

Returns a new data layout for dispatching threadgroups over indirect buffer calls, with specified threadgroups per grid.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
init(threadgroupsPerGrid: (UInt32, UInt32, UInt32))
```

## Parameters 

`threadgroupsPerGrid`  

The number of threadgroups for the grid, in each dimension.

## See Also

### Specifying the Size of the Threadgroup

init()

Returns a new data layout for dispatching threadgroups over indirect buffer calls.

var threadgroupsPerGrid: (UInt32, UInt32, UInt32)

The number of threadgroups for the grid, in each dimension.

