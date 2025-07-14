

- Swift Charts
- ChartContent
-  accessibilityValue(\_:) 

Instance Method

# accessibilityValue(\_:)

Adds a description of the value that the chart content contains.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func accessibilityValue(_ valueDescription: Text) -> some ChartContent
```

## See Also

### Configuring accessibility

func accessibilityHidden(Bool) -> some ChartContent

Specifies whether to hide this chart content from system accessibility features.

func accessibilityIdentifier(String) -> some ChartContent

Adds an identifier string to the chart content.

func accessibilityLabel(LocalizedStringKey) -> some ChartContent

Adds a label to the chart content that describes its contents.

func accessibilityLabel&lt;S>(S) -> some ChartContent

Adds a label to the chart content that describes its contents.

func accessibilityLabel(Text) -> some ChartContent

Adds a label to the chart content that describes its contents.

func accessibilityValue(LocalizedStringKey) -> some ChartContent

Adds a description of the value that the chart content contains.

func accessibilityValue&lt;S>(S) -> some ChartContent

Adds a description of the value that the chart content contains.

