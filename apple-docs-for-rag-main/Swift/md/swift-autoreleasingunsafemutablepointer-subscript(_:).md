

- Swift
- AutoreleasingUnsafeMutablePointer
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Access the `i`th element of the raw array pointed to by `self`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(i: Int) -> Pointee { get }
```

## Overview

Precondition

`self != nil`.

## See Also

### Accessing a Pointer’s Memory

var pointee: Pointee

Retrieve or set the `Pointee` instance referenced by `self`.

