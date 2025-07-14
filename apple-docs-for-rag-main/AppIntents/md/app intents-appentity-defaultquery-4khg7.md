

- App Intents
- AppEntity
-  defaultQuery 

Type Property

# defaultQuery

The default query to use to retrieve entity property instances.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var defaultQuery: Self.DefaultQuery { get }
```

**Required** Default implementations provided.

## Mentioned in 

Integrating custom data types into your intents

## Discussion

You can create a query that uses identifier, name and more. For additional information, see Query.

## Default Implementations

### AppEntity Implementations

static var defaultQuery: _TransientAppEntityQuery&lt;Self>

static var defaultQuery: _RawRepresentableStringQuery&lt;Self>

## See Also

### Making the entity queryable

associatedtype DefaultQuery : EntityQuery

**Required**

static var defaultResolverSpecification: EmptyResolverSpecification&lt;Self>

static var defaultResolverSpecification: some ResolverSpecification

