

- System
- FilePath
- FilePath.Component
-  extension 

Instance Property

# extension

The extension of this file or directory component.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var `extension`: String? { get }
```

## Discussion

If `self` does not contain a `.` anywhere, or only at the start, returns `nil`. Otherwise, returns everything after the dot.

Examples:

- `foo.txt => txt`

- `foo.tar.gz => gz`

- `Foo.app => app`

- `.hidden => nil`

- `.. => nil`

