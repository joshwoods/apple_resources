

- Metal
- MTLBinaryArchiveError
-  unexpectedElement 

Type Property

# unexpectedElement

An error code that indicates a problem with a configuration, typically in a descriptor or an archive’s inability to add linked functions.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
static var unexpectedElement: MTLBinaryArchiveError.Code { get }
```

## See Also

### Error Codes

static var none: MTLBinaryArchiveError.Code

An error code that represents the absence of any problems.

static var invalidFile: MTLBinaryArchiveError.Code

An error code that indicates an app is using an invalid reference to an archive file, typically related to a URL.

static var compilationFailure: MTLBinaryArchiveError.Code

An error code that indicates the archive’s inability to compile its contents, typically when serializing it to a URL.

static var internalError: MTLBinaryArchiveError.Code

An error code that indicates the Metal framework has an internal problem.

enum Code

Error codes when creating binary archives of compiled shader code.

