

- Foundation
- NSExtensionContext
-  completeRequest(withBroadcast:broadcastConfiguration:setupInfo:) Deprecated

Instance Method

# completeRequest(withBroadcast:broadcastConfiguration:setupInfo:)

Tells the host app to complete the app extension request with the specified broadcast information.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 10.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func completeRequest(
    withBroadcast broadcastURL: URL,
    broadcastConfiguration: RPBroadcastConfiguration,
    setupInfo: [String : any NSCoding & NSObjectProtocol]?
)
```

Deprecated

Use completeRequest(withBroadcast:setupInfo:) instead.

## See Also

### Deprecated

var widgetActiveDisplayMode: NCWidgetDisplayMode

The active display mode of the widget.

Deprecated

var widgetLargestAvailableDisplayMode: NCWidgetDisplayMode

The largest display mode the widget supports.

Deprecated

func widgetMaximumSize(for: NCWidgetDisplayMode) -> CGSize

Returns the maximum size for the specified widget display mode.

Deprecated

