

- Swift
- String
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the character at the given position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(i: String.Index) -> Character { get }
```

## Parameters 

`i`  

A valid index of the string. `i` must be less than the string’s end index.

## Overview

You can use the same indices for subscripting a string and its substring. For example, this code finds the first letter after the first space:

```
let str = "Greetings, friend! How are you?"
let firstSpace = str.firstIndex(of: " ") ?? str.endIndex
let substr = str[firstSpace...]
if let nextCapital = substr.firstIndex(where: { $0 >= "A" && $0 

## See Also

### Getting Characters and Bytes

var first: Self.Element?

The first element of the collection.

var last: Self.Element?

The last element of the collection.

func randomElement() -> Self.Element?

Returns a random element of the collection.

func randomElement&lt;T>(using: inout T) -> Self.Element?

Returns a random element of the collection, using the given generator as a source for randomness.

