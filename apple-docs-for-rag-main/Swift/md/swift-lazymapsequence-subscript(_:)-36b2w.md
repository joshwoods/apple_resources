

- Swift
- LazyMapSequence
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the element at `position`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(position: Base.Index) -> Element { get }
```

Available when `Base` conforms to `Collection`.

## Overview

Precondition

`position` is a valid position in `self` and `position != endIndex`.

