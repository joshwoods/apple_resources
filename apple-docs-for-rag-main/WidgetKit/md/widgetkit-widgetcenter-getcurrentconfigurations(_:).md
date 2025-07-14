

- WidgetKit
- WidgetCenter
-  getCurrentConfigurations(\_:) 

Instance Method

# getCurrentConfigurations(\_:)

Retrieves information about user-configured widgets.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
@preconcurrency
func getCurrentConfigurations(_ completion: @escaping (Result) -> Void)
```

## Parameters 

`completion`  

A completion handler called when the widget information is available.

## Mentioned in 

Making a configurable widget

## See Also

### Getting Widget Information

static let shared: WidgetCenter

The shared widget center.

struct UserInfoKey

An object that defines keys for accessing information in a user info dictionary.

