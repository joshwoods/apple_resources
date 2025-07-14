

- Swift
- StringProtocol
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns `true` if `other` is non-empty and contained within `self` by case-sensitive, non-literal search. Otherwise, returns `false`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func contains(_ other: T) -> Bool where T : StringProtocol
```

## Discussion

Equivalent to `self.range(of: other) != nil`

