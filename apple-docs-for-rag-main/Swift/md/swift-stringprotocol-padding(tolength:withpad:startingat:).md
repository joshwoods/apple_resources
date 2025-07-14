

- Swift
- StringProtocol
-  padding(toLength:withPad:startingAt:) 

Instance Method

# padding(toLength:withPad:startingAt:)

Returns a new string formed from the `String` by either removing characters from the end, or by appending as many occurrences as necessary of a given pad string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func padding(
    toLength newLength: Int,
    withPad padString: T,
    startingAt padIndex: Int
) -> String where T : StringProtocol
```

