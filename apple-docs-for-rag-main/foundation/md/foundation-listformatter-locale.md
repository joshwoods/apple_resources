

- Foundation
- ListFormatter
-  locale 

Instance Property

# locale

The locale to use when formatting items in the list.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var locale: Locale! { get set }
```

## Discussion

The default value is autoupdatingCurrent. If you set this property to `nil`, the formatter resets to using autoupdatingCurrent.

## See Also

### Configuring Formatter Options

var itemFormatter: Formatter?

An object that formats each item in the list.

