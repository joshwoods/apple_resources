

- Foundation
- HTTPCookiePropertyKey
-  init(\_:) 

Initializer

# init(\_:)

Creates an HTTP cookie property key using the given string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ rawValue: String)
```

## Parameters 

`rawValue`  

The string to use as a key.

## Discussion

You can use this initializer to create HTTP cookie property keys that aren’t already represented by the predefined constants.

This convenience initializer is identical to init(rawValue:).

## See Also

### Creating custom cookie property keys

init(rawValue: String)

