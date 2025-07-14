

- Swift Charts
- VectorizedChartContent
-  accessibilityHidden(\_:) 

Instance Method

# accessibilityHidden(\_:)

Specifies whether to hide this chart content from system accessibility features.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityHidden(_ hidden: KeyPath) -> some VectorizedChartContent
```

## See Also

### Configuring accessibility

func accessibilityIdentifier(KeyPath&lt;Self.DataElement, String>) -> some VectorizedChartContent&lt;Self.DataElement> 

Adds an identifier string to the chart content.

func accessibilityLabel(KeyPath&lt;Self.DataElement, some StringProtocol>) -> some VectorizedChartContent&lt;Self.DataElement> 

Adds a label to the chart content that describes its contents.

func accessibilityValue(KeyPath&lt;Self.DataElement, some StringProtocol>) -> some VectorizedChartContent&lt;Self.DataElement> 

Adds a description of the value that the chart content contains.

