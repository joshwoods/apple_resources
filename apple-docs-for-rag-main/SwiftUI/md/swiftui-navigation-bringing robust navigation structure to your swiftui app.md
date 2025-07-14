

- SwiftUI
- Navigation
-  Bringing robust navigation structure to your SwiftUI app 

Sample Code

# Bringing robust navigation structure to your SwiftUI app

Use navigation links, stacks, destinations, and paths to provide a streamlined experience for all platforms, as well as behaviors such as deep linking and state restoration.

Download

iOS 18.0+iPadOS 18.0+macOS 15.0+Xcode 16.0+

## Overview

Note

This sample code project is associated with WWDC22 session 10054: The SwiftUI cookbook for navigation.

## See Also

### Presenting views in columns

Migrating to new navigation types

Improve navigation behavior in your app by replacing navigation views with navigation stacks and navigation split views.

struct NavigationSplitView

A view that presents views in two or three columns, where selections in leading columns control presentations in subsequent columns.

func navigationSplitViewStyle&lt;S>(S) -> some View

Sets the style for navigation split views within this view.

func navigationSplitViewColumnWidth(CGFloat) -> some View

Sets a fixed, preferred width for the column containing this view.

func navigationSplitViewColumnWidth(min: CGFloat?, ideal: CGFloat, max: CGFloat?) -> some View

Sets a flexible, preferred width for the column containing this view.

struct NavigationSplitViewVisibility

The visibility of the leading columns in a navigation split view.

struct NavigationLink

A view that controls a navigation presentation.

