

- WidgetKit
-  WidgetRelevanceAttribute 

Structure

# WidgetRelevanceAttribute

A type describing when a specific widget could be relevant.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
struct WidgetRelevanceAttribute
```

## Overview

You use `RelevantContext` as way to describe when a specific widget can be relevant.

## Topics

### Initializers

init(configuration: Configuration, context: RelevantContext)

Creates a new widget relevance for a specific configuration that is relevant in a specific context.

init(configuration: Configuration, context: RelevantContext)

Creates a new widget relevance for a specific configuration that is relevant in a specific context.

init(configuration: Configuration, group: WidgetRelevanceGroup)

Associates the widget kind with a group. When multiple widgets are in the same group, the system will only suggest one member of the group simultaneously. Widgets in the same group are interpreted to contain redundant information, and therefore should not be presented together.

init(configuration: Configuration, group: WidgetRelevanceGroup)

Associates the widget kind with a group. When multiple widgets are in the same group, the system will only suggest one member of the group simultaneously. Widgets in the same group are interpreted to contain redundant information, and therefore should not be presented together.

init(context: RelevantContext)

Creates a new widget relevance that is relevant in a specific context.

init(group: WidgetRelevanceGroup)

Associates the widget kind with a group. When multiple widgets are in the same group, the system will only suggest one member of the group simultaneously. Widgets in the same group are interpreted to contain redundant information, and therefore should not be presented together.

