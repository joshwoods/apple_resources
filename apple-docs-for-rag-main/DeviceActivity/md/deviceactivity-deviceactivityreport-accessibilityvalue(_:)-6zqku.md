

- DeviceActivity
- DeviceActivityReport
-  accessibilityValue(\_:) 

Instance Method

# accessibilityValue(\_:)

Adds a textual description of the value that the view contains.

DeviceActivitySwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func accessibilityValue(_ value: S) -> ModifiedContent where S : StringProtocol
```

## Discussion

Use this method to describe the value represented by a view, but only if that’s different than the view’s label. For example, for a slider that you label as “Volume” using accessibilityLabel(), you can provide the current volume setting, like “60%”, using accessibilityValue().

