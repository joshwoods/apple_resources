

- SwiftUI
- Navigation
- NavigationLink
-  Deprecated symbols 

API Collection

# Deprecated symbols

Review deprecated navigation link initializers.

## Overview

For information about updating your use of navigation symbols, see Migrating to new navigation types.

## Topics

### Creating links with view builders

init(_:isActive:destination:)

Creates a navigation link that presents a destination view when active, with a text label that the link generates from a localized string key.

Deprecated

init(isActive: Binding&lt;Bool>, destination: () -> Destination, label: () -> Label)

Creates a navigation link that presents the destination view when active.

Deprecated

init(_:tag:selection:destination:)

Creates a navigation link that presents a destination view when a bound selection variable matches a value you provide, using a text label that the link generates from a title string.

Deprecated

init&lt;V>(tag: V, selection: Binding&lt;V?>, destination: () -> Destination, label: () -> Label)

Creates a navigation link that presents the destination view when a bound selection variable equals a given tag value.

Deprecated

### Creating links for WatchKit

init(destinationName: String, isActive: Binding&lt;Bool>, label: () -> Label)

Creates a navigation link that presents a view from a WatchKit storyboard when active.

Deprecated

init&lt;V>(destinationName: String, tag: V, selection: Binding&lt;V?>, label: () -> Label)

Creates a navigation link that presents a view from a WatchKit storyboard when a bound selection variable matches a value you provide.

Deprecated

init(destinationName: String, label: () -> Label)

Creates a navigation link that presents a view from a WatchKit storyboard.

Deprecated

### Creating links with view arguments

init(_:destination:isActive:)

Creates a navigation link that presents a destination view when active, with a text label that the link generates from a localized string key.

Deprecated

init(destination: Destination, isActive: Binding&lt;Bool>, label: () -> Label)

Creates a navigation link that presents the destination view when active.

Deprecated

init(_:destination:tag:selection:)

Creates a navigation link that presents a destination view when a bound selection variable matches a value you provide, using a text label that the link generates from a title string.

Deprecated

init&lt;V>(destination: Destination, tag: V, selection: Binding&lt;V?>, label: () -> Label)

Creates a navigation link that presents the destination view when a bound selection variable equals a given tag value.

Deprecated

