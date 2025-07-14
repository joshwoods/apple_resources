

- Metal
- MTLFunctionDescriptor
-  constantValues 

Instance Property

# constantValues

The set of constant values assigned to the function constants.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
@NSCopying
var constantValues: MTLFunctionConstantValues? { get set }
```

## Discussion

The default value is `nil`. If you are creating a function object for a specialized function, you must provide an array of valid constant values for all required function constants.

## See Also

### Specifying the Function Configuration

var name: String?

The name of the function to fetch from the library.

var specializedName: String?

A new name for the created function object.

var options: MTLFunctionOptions

Flags specifying how Metal should create the new function object.

var binaryArchives: [any MTLBinaryArchive]?

The binary archives to search for a previously-compiled version of this function.

struct MTLFunctionOptions

Options that define how Metal creates the function object.

class MTLLinkedFunctions

A set of related functions that Metal links to when necessary to create the function object.

