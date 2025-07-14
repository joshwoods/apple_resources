

- Swift
- AnyBidirectionalCollection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the element indicated by `position`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(position: AnyBidirectionalCollection.Index) -> Element { get }
```

## Overview

Precondition

`position` indicates a valid position in `self` and `position != endIndex`.

