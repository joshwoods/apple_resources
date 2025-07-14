

- System
- FileDescriptor
-  open(\_:\_:options:permissions:retryOnInterrupt:) 

Type Method

# open(\_:\_:options:permissions:retryOnInterrupt:)

Opens or creates a file for reading or writing.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static func open(
    _ path: FilePath,
    _ mode: FileDescriptor.AccessMode,
    options: FileDescriptor.OpenOptions = FileDescriptor.OpenOptions(),
    permissions: FilePermissions? = nil,
    retryOnInterrupt: Bool = true
) throws -> FileDescriptor
```

## Parameters 

`path`  

The location of the file to open.

`mode`  

The read and write access to use.

`options`  

The behavior for opening the file.

`permissions`  

The file permissions to use for created files.

`retryOnInterrupt`  

Whether to retry the open operation if it throws interrupted. The default is `true`. Pass `false` to try only once and throw an error upon interruption.

## Return Value

A file descriptor for the open file

## Discussion

The corresponding C function is `open`.

## See Also

### Opening a File

static func open(UnsafePointer&lt;CChar>, FileDescriptor.AccessMode, options: FileDescriptor.OpenOptions, permissions: FilePermissions?, retryOnInterrupt: Bool) throws -> FileDescriptor

Opens or creates a file for reading or writing.

struct AccessMode

The desired read and write access for a newly opened file.

struct OpenOptions

Options that specify behavior for a newly-opened file.

