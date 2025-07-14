

- Metal
- MTLFunctionDescriptor
-  specializedName 

Instance Property

# specializedName

A new name for the created function object.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var specializedName: String? { get set }
```

## Discussion

The default value is `nil`. If you specify a value for this property, Metal creates the new MTLFunction object with the new name. Use this property if you want to specialize a function with multiple variants and give each a distinct name.

## See Also

### Specifying the Function Configuration

var name: String?

The name of the function to fetch from the library.

var constantValues: MTLFunctionConstantValues?

The set of constant values assigned to the function constants.

var options: MTLFunctionOptions

Flags specifying how Metal should create the new function object.

var binaryArchives: [any MTLBinaryArchive]?

The binary archives to search for a previously-compiled version of this function.

struct MTLFunctionOptions

Options that define how Metal creates the function object.

class MTLLinkedFunctions

A set of related functions that Metal links to when necessary to create the function object.

