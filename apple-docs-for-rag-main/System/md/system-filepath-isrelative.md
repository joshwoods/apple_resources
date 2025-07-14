

- System
- FilePath
-  isRelative 

Instance Property

# isRelative

Returns true if this path is not absolute (see `isAbsolute`).

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var isRelative: Bool { get }
```

## Discussion

Examples:

- Unix:

  - `~/bar`

  - `tmp/foo.txt`

- Windows:

  - `bar\baz`

  - `C:Users\`

  - `\Users`

