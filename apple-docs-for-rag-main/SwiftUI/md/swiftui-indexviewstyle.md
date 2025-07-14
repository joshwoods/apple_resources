

- SwiftUI
-  IndexViewStyle 

Protocol

# IndexViewStyle

Defines the implementation of all `IndexView` instances within a view hierarchy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+watchOS 8.0+

``` source
protocol IndexViewStyle
```

## Overview

To configure the current `IndexViewStyle` for a view hierarchy, use the `.indexViewStyle()` modifier.

## Topics

### Getting built-in index view styles

static var page: PageIndexViewStyle

An index view style that places a page index view over its content.

static func page(backgroundDisplayMode: PageIndexViewStyle.BackgroundDisplayMode) -> PageIndexViewStyle

An index view style that places a page index view over its content.

### Supporting types

struct PageIndexViewStyle

An index view style that places a page index view over its content.

## Relationships

### Conforming Types

- PageIndexViewStyle

## See Also

### Styling groups

func controlGroupStyle&lt;S>(S) -> some View

Sets the style for control groups within this view.

protocol ControlGroupStyle

Defines the implementation of all control groups within a view hierarchy.

struct ControlGroupStyleConfiguration

The properties of a control group.

func formStyle&lt;S>(S) -> some View

Sets the style for forms in a view hierarchy.

protocol FormStyle

The appearance and behavior of a form.

struct FormStyleConfiguration

The properties of a form instance.

func groupBoxStyle&lt;S>(S) -> some View

Sets the style for group boxes within this view.

protocol GroupBoxStyle

A type that specifies the appearance and interaction of all group boxes within a view hierarchy.

struct GroupBoxStyleConfiguration

The properties of a group box instance.

func indexViewStyle&lt;S>(S) -> some View

Sets the style for the index view within the current environment.

func labeledContentStyle&lt;S>(S) -> some View

Sets a style for labeled content.

protocol LabeledContentStyle

The appearance and behavior of a labeled content instance..

struct LabeledContentStyleConfiguration

The properties of a labeled content instance.

