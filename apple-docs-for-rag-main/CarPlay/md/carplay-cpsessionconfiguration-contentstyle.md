

- CarPlay
- CPSessionConfiguration
-  contentStyle 

Instance Property

# contentStyle

The content style that the vehicle selects.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var contentStyle: CPContentStyle { get }
```

## Discussion

The vehicle selects the content style according to the ambient light level. Your navigation app can use this value to determine the most appropriate style of map content to draw in its base view. The content style is independent of the user interface style, which controls light and dark mode.

## See Also

### Getting the Content Style

struct CPContentStyle

The types of content style that the vehicle allows.

