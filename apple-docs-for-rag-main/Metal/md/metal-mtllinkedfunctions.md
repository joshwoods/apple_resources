

- Metal
-  MTLLinkedFunctions 

Class

# MTLLinkedFunctions

A set of related functions that Metal links to when necessary to create the function object.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MTLLinkedFunctions
```

## Overview

When you create a Metal function object using a MTLFunctionDescriptor, you specify additional functions that Metal needs to link to when it compiles and links the underlying shader code. Most often, you need to do this if your shader takes a visible function table as one or more of its arguments. For Metal to create the MTLFunction object, it needs a complete list of functions that your shader can call so that it can resolve any dependencies and generate the correct code to run on the GPU.

## Topics

### Specifying Related Functions

var functions: [any MTLFunction]?

An array of function objects to link to the new function.

var binaryFunctions: [any MTLFunction]?

An array of function objects already compiled to a binary representation to link.

var groups: [String : [any MTLFunction]]?

An optional list of groups specifying which functions your shader can call at each call site.

var privateFunctions: [any MTLFunction]?

An array of function objects to link to the new function, without exporting the functions publicly.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

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

var binaryArchives: [any MTLBinaryArchive]?

The binary archives to search for a previously-compiled version of this function.

struct MTLFunctionOptions

Options that define how Metal creates the function object.

