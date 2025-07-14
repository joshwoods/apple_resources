

- Foundation
- NSExtensionContext
-  widgetLargestAvailableDisplayMode Deprecated

Instance Property

# widgetLargestAvailableDisplayMode

The largest display mode the widget supports.

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0Deprecated

``` source
var widgetLargestAvailableDisplayMode: NCWidgetDisplayMode { get set }
```

Deprecated

Use WidgetKit instead.

## Discussion

The default value of this property is NCWidgetDisplayMode.compact. At any time, you can change the largest display mode your widget supports by changing the value of this property. For example, you can update the property value as more or less content is available to display in your widget.

## See Also

### Deprecated

func completeRequest(withBroadcast: URL, broadcastConfiguration: RPBroadcastConfiguration, setupInfo: [String : any NSCoding &amp; NSObjectProtocol]?)

Tells the host app to complete the app extension request with the specified broadcast information.

Deprecated

var widgetActiveDisplayMode: NCWidgetDisplayMode

The active display mode of the widget.

Deprecated

func widgetMaximumSize(for: NCWidgetDisplayMode) -> CGSize

Returns the maximum size for the specified widget display mode.

Deprecated

