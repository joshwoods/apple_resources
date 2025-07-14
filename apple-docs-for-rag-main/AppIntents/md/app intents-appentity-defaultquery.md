

- App Intents
- AppEntity
-  DefaultQuery 

Associated Type

# DefaultQuery

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
associatedtype DefaultQuery : EntityQuery where Self.ValueType == Self.DefaultQuery.Entity
```

**Required**

## See Also

### Making the entity queryable

static var defaultQuery: Self.DefaultQuery

The default query to use to retrieve entity property instances.

**Required** Default implementations provided.

static var defaultResolverSpecification: EmptyResolverSpecification&lt;Self>

static var defaultResolverSpecification: some ResolverSpecification

