

- WidgetKit
-  WidgetRelevance 

Structure

# WidgetRelevance

A type collecting the relevances for a widget kind.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
struct WidgetRelevance
```

## Overview

Return this type from either `TimelineProvider.relevances()`, `AppIntentTimelineProvider.relevances()` or `IntentTimelineProvider.relevances` to inform the system of when a widget might be relevant and in which configuration.

Make sure to return the relevances in priority order because the system might decide to utilize only a subset of the provided relevances.

## Topics

### Initializers

init([WidgetRelevanceAttribute&lt;Configuration>])

Creates a type collecting the relevances for a widget kind.

