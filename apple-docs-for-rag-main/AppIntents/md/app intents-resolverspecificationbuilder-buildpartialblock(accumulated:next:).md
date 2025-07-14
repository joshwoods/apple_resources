

- App Intents
- ResolverSpecificationBuilder
-  buildPartialBlock(accumulated:next:) 

Type Method

# buildPartialBlock(accumulated:next:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func buildPartialBlock(
    accumulated: ResolverSpecificationBuilder.Specification,
    next: R
) -> ResolverSpecificationBuilder.Specification where repeat each Accumulated : Resolver, R : Resolver
```

Available when `Property` conforms to `_IntentValue`.

