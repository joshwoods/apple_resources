

- App Intents
- ResolverSpecificationBuilder
-  buildExpression(\_:) 

Type Method

# buildExpression(\_:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@backDeployed(before: macOS 15.0, iOS 18.0, watchOS 11.0, tvOS 18.0, visionOS 2.0)
static func buildExpression(_ expression: ResolverType) -> ResolverType where Property == ResolverType.Output, ResolverType : Resolver
```

Available when `Property` conforms to `_IntentValue`.

