

- Swift
-  MirrorPath 

Protocol

# MirrorPath

A protocol for legitimate arguments to `Mirror`’s `descendant` method.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol MirrorPath
```

## Overview

Do not declare new conformances to this protocol; they will not work as expected.

## Relationships

### Conforming Types

- Int
- String

## See Also

### Querying Descendants

func descendant(any MirrorPath, any MirrorPath...) -> Any?

Returns a specific descendant of the reflected subject, or `nil` if no such descendant exists.

