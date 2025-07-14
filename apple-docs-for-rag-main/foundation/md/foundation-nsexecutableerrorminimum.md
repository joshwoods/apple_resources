

- Foundation
-  NSExecutableErrorMinimum 

Global Variable

# NSExecutableErrorMinimum

The beginning of the range of error codes reserved for errors related to executable files.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var NSExecutableErrorMinimum: Int { get }
```

## See Also

### Errors

var NSExecutableNotLoadableError: Int

The executable type isn’t loadable in the current process.

var NSExecutableArchitectureMismatchError: Int

The executable doesn’t provide an architecture compatible with the current process.

var NSExecutableRuntimeMismatchError: Int

The executable has Objective-C runtime information that’s incompatible with the current process.

var NSExecutableLoadError: Int

Executable cannot be loaded for an otherwise-unspecified reason.

var NSExecutableLinkError: Int

The executable failed due to linking issues.

var NSExecutableErrorMaximum: Int

The end of the range of error codes reserved for errors related to executable files.

