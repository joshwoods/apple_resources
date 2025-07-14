

- Metal
- MTLDynamicLibrary
-  serialize(to:) 

Instance Method

# serialize(to:)

Writes the contents of the dynamic library to a file.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func serialize(to url: URL) throws
```

**Required**

## Parameters 

`url`  

The URL for the destination file.

## Discussion

When the methods succeeds, the file contains a representation of the MTLLibrary from the MTLDynamicLibrary that creates it, as well as the binaries it has for the device your app is running on.

Such files may be combined with offline tools to contain the compiled code for multiple devices.

If this MTLDynamicLibrary was created from a file that contained compiled code for multiple devices, the compiled code for all other devices is not written (since only compiled code for the current device was loaded).

