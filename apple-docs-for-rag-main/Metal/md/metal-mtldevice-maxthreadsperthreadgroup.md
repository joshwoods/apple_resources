

- Metal
- MTLDevice
-  maxThreadsPerThreadgroup 

Instance Property

# maxThreadsPerThreadgroup

The maximum number of threads along each dimension of a threadgroup.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var maxThreadsPerThreadgroup: MTLSize { get }
```

**Required**

## Discussion

This size isn’t guaranteed for all shaders. The number of trival shaders supported at once on device determines this value. For more accurate information on the allowable maximum threads per threadgroup in an individual pass, inspect your associated pipeline state.

For more information on the specific threadgroup limits of each GPU family, see the Metal feature set tables:

- Metal feature set tables (PDF)

- Metal feature set tables (Numbers)

## See Also

### Checking Compute Support

var maxThreadgroupMemoryLength: Int

The maximum threadgroup memory available to a compute kernel, in bytes.

**Required**

