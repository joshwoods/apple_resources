

- Foundation
- NSArray
-  pathsMatchingExtensions(\_:) 

Instance Method

# pathsMatchingExtensions(\_:)

Returns an array containing all the pathname elements in the receiving array that have filename extensions from a given array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func pathsMatchingExtensions(_ filterTypes: [String]) -> [String]
```

## Parameters 

`filterTypes`  

An array of `NSString` objects containing filename extensions. The extensions should not include the dot (”.”) character.

## Return Value

An array containing all the pathname elements in the receiving array that have filename extensions from the `filterTypes` array.

