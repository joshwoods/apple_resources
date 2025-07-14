

- App Intents
- EntityQueryProperty
-  init(\_:entityProvider:comparators:) 

Initializer

# init(\_:entityProvider:comparators:)

Initializes a EntityQueryProperty that applies to entity property at the provided keyPath.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    _ keyPath: KeyPath,
    entityProvider: @escaping (Entity) -> Subject,
    @EntityQueryComparatorsBuilder comparators: () -> EntityQueryProperty.QueryComparators
)
```

## Parameters 

`keyPath`  

The keypath to the property that this EntityQueryProperty applies to. The target property type determines which comparator modifiers will be available.

`entityProvider`  

Closure which, given a `Entity` instance, returns the appropriate `Subject` instance to apply `EntityQueryComparator`s to.

`comparators`  

The set of `EntityQueryComparators` that this property supports being queried by.

