

- App Intents
-  IntentItemSection 

Structure

# IntentItemSection

An object you use to divide dynamic options into sections.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentItemSection where Result : _IntentValue
```

## Overview

The system returns an `IntentItemSection` within an IntentItemCollection.

## Topics

### Initializers

init(LocalizedStringResource, items: [Result])

init(LocalizedStringResource, items: [IntentItem&lt;Result>])

init(LocalizedStringResource?, itemsBuilder: () -> [IntentItem&lt;Result>])

init(LocalizedStringResource, subtitle: LocalizedStringResource?, image: DisplayRepresentation.Image?, itemsBuilder: () -> [IntentItem&lt;Result>])

init(items: [IntentItem&lt;Result>])

init(title: LocalizedStringResource, items: [IntentItem&lt;Result>])Deprecated

### Instance Properties

var description: DisplayRepresentation?

var items: [IntentItem&lt;Result>]

### Enumerations

enum Builder

## See Also

### Items and collections

struct IntentItem

A type describing a value returned from a dynamic options provider, plus information about how to display it to users.

struct IntentItemCollection

Return this object to provide an advanced list of options, optionally divided in sections.

struct IntentCollectionSize

