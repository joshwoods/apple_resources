

- App Intents
- EntityQueryProperty
-  init(\_:comparators:) 

Initializer

# init(\_:comparators:)

Initializes a EntityQueryProperty that applies to entity property at the provided keyPath.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
convenience init(
    _ keyPath: KeyPath,
    @EntityQueryComparatorsBuilder comparators: () -> EntityQueryProperty.QueryComparators
) where Entity == Subject
```

## Parameters 

`keyPath`  

The keypath to the property that this EntityQueryProperty applies to. The target property type determines which comparator modifiers will be available.

`comparators`  

The set of `EntityQueryComparators` that this property supports being queried by.

