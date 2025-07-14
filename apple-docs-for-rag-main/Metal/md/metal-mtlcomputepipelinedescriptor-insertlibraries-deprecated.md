

- Metal
- MTLComputePipelineDescriptor
-  insertLibraries Deprecated

Instance Property

# insertLibraries

The dynamic libraries that contain precompiled shader functions you want to link.

iOS 14.0–15.0DeprecatediPadOS 14.0–15.0DeprecatedMac Catalyst 14.0–15.0DeprecatedmacOS 11.0–12.0DeprecatedtvOS 14.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var insertLibraries: [any MTLDynamicLibrary]? { get set }
```

Deprecated

Use the preloadedLibraries property instead.

## See Also

### Loading Dynamic Libraries to Link at Runtime

var preloadedLibraries: [any MTLDynamicLibrary]

The dynamic libraries that contain precompiled shader functions you want to link.

