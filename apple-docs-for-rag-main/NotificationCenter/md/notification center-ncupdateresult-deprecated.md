

- Notification Center
-  NCUpdateResult Deprecated

Enumeration

# NCUpdateResult

The result of updating a widget’s state.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 8.0–14.0DeprecatedmacOS 10.10–11.0Deprecated

``` source
enum NCUpdateResult
```

Deprecated

Use WidgetKit instead.

## Topics

### Constants

case newData

The update resulted in new data to display.

case noData

The update did not result in any new data since the last update.

case failed

The update attempt failed.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Updating a Widget’s Contents

func widgetPerformUpdate(completionHandler: (NCUpdateResult) -> Void)

Called to give a widget an opportunity to update its contents.

Deprecated

