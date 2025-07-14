

- App Intents
-  IntentItem 

Structure

# IntentItem

A type describing a value returned from a dynamic options provider, plus information about how to display it to users.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentItem where Value : _IntentValue
```

## Topics

### Initializers

init(Value)

Initialize an `IntentItem` and use `displayRepresentation` from `value`

init(Value, title: LocalizedStringResource, subtitle: LocalizedStringResource?, image: DisplayRepresentation.Image?)

Creates an item with the specified value and visual attributes.

### Instance Properties

var description: DisplayRepresentation

var value: Value

### Enumerations

enum Builder

## See Also

### Items and collections

struct IntentItemCollection

Return this object to provide an advanced list of options, optionally divided in sections.

struct IntentItemSection

An object you use to divide dynamic options into sections.

struct IntentCollectionSize

