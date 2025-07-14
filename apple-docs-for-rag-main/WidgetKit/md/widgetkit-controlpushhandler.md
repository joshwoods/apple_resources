

- WidgetKit
-  ControlPushHandler 

Protocol

# ControlPushHandler

A type that can receive push information about user-configured controls.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
protocol ControlPushHandler
```

## Overview

Register a type conforming to this protocol to receive push information using the `ControlWidgetConfiguration/pushHandler(_:)` modifier on your controls’ configurations.

## Topics

### Initializers

init()

Creates a push handler.

**Required**

### Instance Methods

func pushTokensDidChange(controls: [ControlInfo])

Handle push tokens changing for configured controls.

**Required**

## See Also

### Control updates

Updating controls locally and remotely

Update and reload controls from your app or using push notifications.

struct ControlPushInfo

A structure that contains information about the push token of a user-configured control.

