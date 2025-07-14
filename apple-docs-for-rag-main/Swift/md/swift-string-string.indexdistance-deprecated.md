

- Swift
- String
-  String.IndexDistance Deprecated

Type Alias

# String.IndexDistance

A type that represents the number of steps between two `String.Index` values, where one value is reachable from the other.

iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+iOS 8.0+

``` source
typealias IndexDistance = Int
```

Deprecated

All index distances are now of type Int

## Discussion

In Swift, *reachability* refers to the ability to produce one value from the other through zero or more applications of `index(after:)`.

