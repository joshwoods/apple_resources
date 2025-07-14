

- System
- FilePath
-  lexicallyNormalize() 

Instance Method

# lexicallyNormalize()

Collapse `.` and `..` components lexically (i.e. without following symlinks).

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func lexicallyNormalize()
```

## Discussion

Examples:

- `/usr/./local/bin/.. => /usr/local`

- `/../usr/local/bin => /usr/local/bin`

- `../usr/local/../bin => ../usr/bin`

