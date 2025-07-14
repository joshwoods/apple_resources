

- Metal
- MTLDispatchThreadgroupsIndirectArguments
-  init() 

Initializer

# init()

Returns a new data layout for dispatching threadgroups over indirect buffer calls.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
init()
```

## See Also

### Specifying the Size of the Threadgroup

init(threadgroupsPerGrid: (UInt32, UInt32, UInt32))

Returns a new data layout for dispatching threadgroups over indirect buffer calls, with specified threadgroups per grid.

var threadgroupsPerGrid: (UInt32, UInt32, UInt32)

The number of threadgroups for the grid, in each dimension.

