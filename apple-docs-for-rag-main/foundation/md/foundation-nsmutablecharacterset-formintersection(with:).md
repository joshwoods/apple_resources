

- Foundation
- NSMutableCharacterSet
-  formIntersection(with:) 

Instance Method

# formIntersection(with:)

Modifies the receiver so it contains only characters that exist in both the receiver and another set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func formIntersection(with otherSet: CharacterSet)
```

## Parameters 

`otherSet`  

The character set with which to perform the intersection.

## See Also

### Combining Character Sets

func formUnion(with: CharacterSet)

Modifies the receiver so it contains all characters that exist in either the receiver or another set.

