

- App Intents
- ContainsComparator
-  init(withResolvers:mappingTransform:) 

Initializer

# init(withResolvers:mappingTransform:)

Declares support for the `contains` operator between a `AttributedString` property and user-supplied values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    @ResolverSpecificationBuilder withResolvers resolvers: @escaping () -> Spec,
    mappingTransform: @escaping (InputType) -> ComparatorMappingType
) where Property : EntityProperty, PropertyType == AttributedString, InputType == AttributedString, Spec : ResolverSpecification
```

## Parameters 

`resolvers`  

Set of `Resolver`s to apply when converting user input to the target `Value` type.

`mappingTransform`  

Closure that transforms the user-supplied value into the `ComparatorMappingType` output type.

