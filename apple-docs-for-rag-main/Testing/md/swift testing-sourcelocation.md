

- Swift Testing
-  SourceLocation 

Structure

# SourceLocation

A type representing a location in source code.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
struct SourceLocation
```

## Topics

### Initializers

init(fileID: String, filePath: String, line: Int, column: Int)

Initialize an instance of this type with the specified location details.

### Instance Properties

var column: Int

The column in the source file.

var fileID: String

The file ID of the source file.

var fileName: String

The name of the source file.

var line: Int

The line in the source file.

var moduleName: String

The name of the module containing the source file.

### Default Implementations

Comparable Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Comparable
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

