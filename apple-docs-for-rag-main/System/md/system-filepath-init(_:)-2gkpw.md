

- System
- FilePath
-  init(\_:) 

Initializer

# init(\_:)

Creates a file path from a URL

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init?(_ url: URL)
```

## Discussion

The result is nil if `url` doesn’t refer to a local file.

