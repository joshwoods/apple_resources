

- AppKit
- NSWorkspace
-  NSWorkspace.FileOperationName Deprecated

Structure

# NSWorkspace.FileOperationName

These constants specify different types of file operations used by performFileOperation(_:source:destination:files:tag:).

macOS 10.0–10.11Deprecated

``` source
struct FileOperationName
```

Deprecated

Use FileManager methods instead.

## Topics

### Type Properties

static let compressOperation: NSWorkspace.FileOperationName

Compress file. This operation always returns an error.

static let copyOperation: NSWorkspace.FileOperationName

Copy file to destination. Behaves the same as copyPath:toPath:handler:.

static let decompressOperation: NSWorkspace.FileOperationName

Decompress file. This operation always returns an error.

static let decryptOperation: NSWorkspace.FileOperationName

Decrypt file. This operation always returns an error.

static let destroyOperation: NSWorkspace.FileOperationName

Destroy file. Behaves the same as removeFileAtPath:handler:.

static let duplicateOperation: NSWorkspace.FileOperationName

Duplicate file in source directory.

static let encryptOperation: NSWorkspace.FileOperationName

Encrypt file. This operation always returns an error.

static let linkOperation: NSWorkspace.FileOperationName

Create hard link to file in destination. Behaves the same as linkPath:toPath:handler:.

static let moveOperation: NSWorkspace.FileOperationName

Move file to destination. Behaves the same as movePath:toPath:handler:.

static let recycleOperation: NSWorkspace.FileOperationName

Move file to trash. The file is moved to the trash folder on the volume containing the file using the same semantics as `NSWorkspaceMoveOperation`. If a file with the same name currently exists in the trash folder, the new file is renamed. If no trash folder exists on the volume containing the file, the operation fails.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Types

struct LaunchOptions

Constants specifying how you want to launch an app

struct LaunchConfigurationKey

The following keys can be used in the configuration dictionary of the launchApplication(at:options:configuration:) method. Each key is optional, and if omitted, default behavior is applied.

Deprecated

