

- Swift Charts
- VectorizedChartContent
-  accessibilityIdentifier(\_:) 

Instance Method

# accessibilityIdentifier(\_:)

Adds an identifier string to the chart content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityIdentifier(_ identifier: KeyPath) -> some VectorizedChartContent
```

## See Also

### Configuring accessibility

func accessibilityHidden(KeyPath&lt;Self.DataElement, Bool>) -> some VectorizedChartContent&lt;Self.DataElement> 

Specifies whether to hide this chart content from system accessibility features.

func accessibilityLabel(KeyPath&lt;Self.DataElement, some StringProtocol>) -> some VectorizedChartContent&lt;Self.DataElement> 

Adds a label to the chart content that describes its contents.

func accessibilityValue(KeyPath&lt;Self.DataElement, some StringProtocol>) -> some VectorizedChartContent&lt;Self.DataElement> 

Adds a description of the value that the chart content contains.

