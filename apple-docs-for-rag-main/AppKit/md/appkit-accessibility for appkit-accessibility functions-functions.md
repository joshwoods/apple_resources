

- AppKit
- Accessibility for AppKit
-  Accessibility Functions 

API Collection

# Accessibility Functions

Global accessibility functions for custom views and controls.

## Overview

Use these NSAccessibility functions to enhance the accessibility experience of your custom view or control. Standard AppKit elements handle this behavior for you.

### Notifications

Your custom view or control may need to let the assistive app know when changes occur. For example, if your control’s value changes, you need to send a valueChanged notification.

NSAccessibility.Notification defines a number of notifications that you can send using the post(element:notification:) method. You typically need to send your own notifications only when you’re creating a custom control or when you’re using a standard control in a nonstandard way. Make sure you’re posting any relevant notifications as your control’s state changes.

## Topics

### Notifications

static func post(element: Any, notification: NSAccessibility.Notification)

Sends a notification to any observing assistive apps.

static func post(element: Any, notification: NSAccessibility.Notification, userInfo: [NSAccessibility.NotificationUserInfoKey : Any]?)

Sends a notification and an optional user info dictionary to any observing assistive apps.

struct Notification

The name of the notification.

struct NotificationUserInfoKey

The key in the user info dictionary for a notification.

### Screen Coordinates

static func screenRect(fromView: NSView, rect: NSRect) -> NSRect

Returns the frame in screen coordinates.

static func screenPoint(fromView: NSView, point: NSPoint) -> NSPoint

Returns the point in screen coordinates.

### Accessibility Objects

static func unignoredChildren(from: [Any]) -> [Any]

Returns a list of unignored accessibility objects, descending the hierarchy, if necessary.

static func unignoredChildrenForOnlyChild(from: Any) -> [Any]

Returns a list of unignored accessibility objects, descending the hierarchy, if necessary.

static func unignoredDescendant(of: Any) -> Any?

Returns an unignored accessibility object, descending the hierarchy, if necessary.

static func unignoredAncestor(of: Any) -> Any?

Returns an unignored accessibility object, ascending the hierarchy, if necessary.

### Protected Content

static func setMayContainProtectedContent(Bool) -> Bool

Sets whether the app may have protected content.

### Descriptions

var description: String?

Returns a standard description for an action.

func description(with: NSAccessibility.Subrole?) -> String?

Returns a standard description for a role and subrole.

static func description(for: Any) -> String?

Returns a standard role description for a user interface element.

## See Also

### Custom View Subclasses

Custom Controls

Support accessibility for custom user interface elements by adopting a role-specific protocol and implementing its methods.

