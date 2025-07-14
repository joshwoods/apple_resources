

- Swift
- String
- String.UTF16View
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the code unit at the given position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(idx: String.UTF16View.Index) -> UTF16.CodeUnit { get }
```

## Overview

The following example uses the subscript to print the value of a string’s first UTF-16 code unit.

```
let greeting = "Hello, friend!"
let i = greeting.utf16.startIndex
print("First character's UTF-16 code unit: \(greeting.utf16[i])")
// Prints "First character's UTF-16 code unit: 72"
```

