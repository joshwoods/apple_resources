

- Metal
- MTLDispatchThreadgroupsIndirectArguments
-  threadgroupsPerGrid 

Instance Property

# threadgroupsPerGrid

The number of threadgroups for the grid, in each dimension.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var threadgroupsPerGrid: (UInt32, UInt32, UInt32)
```

## See Also

### Specifying the Size of the Threadgroup

init()

Returns a new data layout for dispatching threadgroups over indirect buffer calls.

init(threadgroupsPerGrid: (UInt32, UInt32, UInt32))

Returns a new data layout for dispatching threadgroups over indirect buffer calls, with specified threadgroups per grid.

