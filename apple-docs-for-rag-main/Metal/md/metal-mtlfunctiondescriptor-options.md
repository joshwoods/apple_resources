

- Metal
- MTLFunctionDescriptor
-  options 

Instance Property

# options

Flags specifying how Metal should create the new function object.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var options: MTLFunctionOptions { get set }
```

## See Also

### Specifying the Function Configuration

var name: String?

The name of the function to fetch from the library.

var specializedName: String?

A new name for the created function object.

var constantValues: MTLFunctionConstantValues?

The set of constant values assigned to the function constants.

var binaryArchives: [any MTLBinaryArchive]?

The binary archives to search for a previously-compiled version of this function.

struct MTLFunctionOptions

Options that define how Metal creates the function object.

class MTLLinkedFunctions

A set of related functions that Metal links to when necessary to create the function object.

