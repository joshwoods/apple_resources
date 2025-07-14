

- SwiftUI
-  SidebarRowSize 

Enumeration

# SidebarRowSize

The standard sizes of sidebar rows.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum SidebarRowSize
```

## Overview

On macOS, sidebar rows have three different sizes: small, medium, and large. The size is primarily controlled by the current users’ “Sidebar Icon Size” in Appearance settings, and applies to all applications.

On all other platforms, the only supported sidebar size is `.medium`.

This size can be read or written in the environment using `EnvironmentValues.sidebarRowSize`.

## Topics

### Getting row sizes

case small

The standard “small” row size

case medium

The standard “medium” row size

case large

The standard “large” row size

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Configuring the sidebar

var sidebarRowSize: SidebarRowSize

The current size of sidebar rows.

