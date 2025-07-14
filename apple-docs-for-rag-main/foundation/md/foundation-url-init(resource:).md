

- Foundation
- URL
-  init(resource:) 

Initializer

# init(resource:)

Creates a URL from a resource.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init?(resource: URLResource)
```

## Parameters 

`resource`  

A URLResource that provides a reference to a resource in a given bundle.

## Discussion

Use this initializer to resolve URLResource instances, possibly received from other processes, into URL instances.

