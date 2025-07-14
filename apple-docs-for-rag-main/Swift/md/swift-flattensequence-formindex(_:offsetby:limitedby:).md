

- Swift
- FlattenSequence
-  formIndex(\_:offsetBy:limitedBy:) 

Instance Method

# formIndex(\_:offsetBy:limitedBy:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func formIndex(
    _ i: inout FlattenSequence.Index,
    offsetBy n: Int,
    limitedBy limit: FlattenSequence.Index
) -> Bool
```

Available when `Base` conforms to `Collection` and `Base.Element` conforms to `Collection`.

