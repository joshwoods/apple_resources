

- Swift
- String
- String.UnicodeScalarView
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the Unicode scalar value at the given position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(position: String.UnicodeScalarView.Index) -> Unicode.Scalar { get }
```

## Parameters 

`position`  

A valid index of the character view. `position` must be less than the view’s end index.

## Overview

The following example searches a string’s Unicode scalars view for a capital letter and then prints the character and Unicode scalar value at the found index:

```
let greeting = "Hello, friend!"
if let i = greeting.unicodeScalars.firstIndex(where: { "A"..."Z" ~= $0 }) {
    print("First capital letter: \(greeting.unicodeScalars[i])")
    print("Unicode scalar value: \(greeting.unicodeScalars[i].value)")
}
// Prints "First capital letter: H"
// Prints "Unicode scalar value: 72"
```

