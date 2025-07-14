

- WidgetKit
- WidgetCenter
-  WidgetCenter.UserInfoKey 

Structure

# WidgetCenter.UserInfoKey

An object that defines keys for accessing information in a user info dictionary.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
struct UserInfoKey
```

## Overview

Note

In Objective-C, use WGWidgetUserInfoKeyFamily and WGWidgetUserInfoKeyKind instead.

## Topics

### Describing a widget

static let family: String

A key you use to access the widget’s family.

static let kind: String

A key you use to access the widget’s kind. The value matches the `kind` property specified in the widget’s configuration.

### Describing a Live Activity

static let activityID: String

A key you use to access the activity ID if the widget represents a Live Activity.

## See Also

### Getting Widget Information

static let shared: WidgetCenter

The shared widget center.

func getCurrentConfigurations((Result&lt;[WidgetInfo], any Error>) -> Void)

Retrieves information about user-configured widgets.

