

- Swift Charts
- ChartContent
-  symbol(\_:) 

Instance Method

# symbol(\_:)

Sets a plotting symbol type for the chart content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func symbol(_ symbol: S) -> some ChartContent where S : ChartSymbolShape
```

## Parameters 

`symbol`  

The symbol.

## See Also

### Setting symbol appearance

func symbol&lt;V>(symbol: () -> V) -> some ChartContent

Sets a SwiftUI view to use as the symbol for the chart content.

func symbolSize(CGSize) -> some ChartContent

Sets the plotting symbol size for the chart content.

func symbolSize(CGFloat) -> some ChartContent

Sets the plotting symbol size for the chart content according to a perceived area.

