

- Foundation
- NSProxy
-  responds(to:) 

Type Method

# responds(to:)

Returns a Boolean value that indicates whether the receiving class responds to a given selector.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func responds(to aSelector: Selector) -> Bool
```

## Parameters 

`aSelector`  

A selector.

## Return Value

true if the receiving class responds to `aSelector` messages, otherwise false.

