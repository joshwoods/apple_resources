

- System
- FilePath
-  lexicallyNormalized() 

Instance Method

# lexicallyNormalized()

Returns a copy of `self` in lexical-normal form, that is `.` and `..` components have been collapsed lexically (i.e. without following symlinks). See `lexicallyNormalize`

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func lexicallyNormalized() -> FilePath
```

