

- Metal
- MTLBinaryArchiveError
-  internalError 

Type Property

# internalError

An error code that indicates the Metal framework has an internal problem.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
static var internalError: MTLBinaryArchiveError.Code { get }
```

## Discussion

You can report the scenario that generated this error code with Feedback Assistant.

## See Also

### Error Codes

static var none: MTLBinaryArchiveError.Code

An error code that represents the absence of any problems.

static var invalidFile: MTLBinaryArchiveError.Code

An error code that indicates an app is using an invalid reference to an archive file, typically related to a URL.

static var compilationFailure: MTLBinaryArchiveError.Code

An error code that indicates the archive’s inability to compile its contents, typically when serializing it to a URL.

static var unexpectedElement: MTLBinaryArchiveError.Code

An error code that indicates a problem with a configuration, typically in a descriptor or an archive’s inability to add linked functions.

enum Code

Error codes when creating binary archives of compiled shader code.

