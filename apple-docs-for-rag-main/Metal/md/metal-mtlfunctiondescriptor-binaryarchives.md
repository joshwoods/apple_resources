

- Metal
- MTLFunctionDescriptor
-  binaryArchives 

Instance Property

# binaryArchives

The binary archives to search for a previously-compiled version of this function.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var binaryArchives: [any MTLBinaryArchive]? { get set }
```

## Mentioned in 

Compiling Binary Archives from a Custom Configuration Script

## Discussion

If you specify an archive that includes a fully compiled version of this function, Metal uses the compiled version rather than creating a new one.

## See Also

### Specifying the Function Configuration

var name: String?

The name of the function to fetch from the library.

var specializedName: String?

A new name for the created function object.

var constantValues: MTLFunctionConstantValues?

The set of constant values assigned to the function constants.

var options: MTLFunctionOptions

Flags specifying how Metal should create the new function object.

struct MTLFunctionOptions

Options that define how Metal creates the function object.

class MTLLinkedFunctions

A set of related functions that Metal links to when necessary to create the function object.

