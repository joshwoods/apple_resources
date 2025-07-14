

- Metal
- MTLLibrary
-  functionNames 

Instance Property

# functionNames

The names of all public functions in the library.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var functionNames: [String] { get }
```

**Required**

## Discussion

Inside a Metal library, functions with the `vertex`, `fragment`, or `kernel` function attributes are entry points into the library. Functions without these attributes are private.

