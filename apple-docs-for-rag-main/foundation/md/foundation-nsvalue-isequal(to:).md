

- Foundation
- NSValue
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Returns a Boolean value that indicates whether the value object and another value object are equal.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isEqual(to value: NSValue) -> Bool
```

## Parameters 

`value`  

The other value object with which to compare the value object.

## Return Value

true if both value objects are equal; otherwise, false.

## Discussion

The NSValue class compares the type and contents of each value object to determine equality.

