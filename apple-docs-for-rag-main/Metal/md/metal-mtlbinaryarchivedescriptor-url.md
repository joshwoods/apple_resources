

- Metal
- MTLBinaryArchiveDescriptor
-  url 

Instance Property

# url

A URL to a Metal binary archive file.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var url: URL? { get set }
```

## Mentioned in 

Creating Binary Archives from Device-Built Pipeline State Objects

## Discussion

You can use this method to load a binary archive you created with an MTLBinaryArchive instance’s serialize(to:) method.

