

- App Intents
-  ResolverSpecificationBuilder 

Enumeration

# ResolverSpecificationBuilder

A result builder that declaratively specifies a set of resolvers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@resultBuilder
enum ResolverSpecificationBuilder where Property : _IntentValue
```

## Topics

### Building the resolver specification

static func buildBlock() -> some ResolverSpecification

static func buildBlock&lt;R0>(R0) -> some ResolverSpecification

static func buildBlock&lt;R0, R1>(R0, R1) -> some ResolverSpecification

static func buildBlock&lt;R0, R1, R2>(R0, R1, R2) -> some ResolverSpecification

static func buildBlock&lt;R0, R1, R2, R3>(R0, R1, R2, R3) -> some ResolverSpecification

static func buildBlock&lt;R0, R1, R2, R3, R4>(R0, R1, R2, R3, R4) -> some ResolverSpecification

static func buildBlock&lt;R0, R1, R2, R3, R4, R5>(R0, R1, R2, R3, R4, R5) -> some ResolverSpecification

static func buildBlock&lt;R0, R1, R2, R3, R4, R5, R6>(R0, R1, R2, R3, R4, R5, R6) -> some ResolverSpecification

static func buildBlock&lt;R0, R1, R2, R3, R4, R5, R6, R7>(R0, R1, R2, R3, R4, R5, R6, R7) -> some ResolverSpecification

static func buildBlock&lt;R0, R1, R2, R3, R4, R5, R6, R7, R8>(R0, R1, R2, R3, R4, R5, R6, R7, R8) -> some ResolverSpecification

### Structures

struct Specification

### Type Methods

static func buildBlock&lt;R0, R1, R2, R3, R4, R5, R6, R7, R8, R9>(R0, R1, R2, R3, R4, R5, R6, R7, R8, R9) -> some ResolverSpecification

static func buildBlock&lt;R0, R1, R2, R3, R4, R5, R6, R7, R8, R9, R10>(R0, R1, R2, R3, R4, R5, R6, R7, R8, R9, R10) -> some ResolverSpecification

static func buildBlock&lt;R0, R1, R2, R3, R4, R5, R6, R7, R8, R9, R10, R11>(R0, R1, R2, R3, R4, R5, R6, R7, R8, R9, R10, R11) -> some ResolverSpecification

static func buildBlock&lt;R0, R1, R2, R3, R4, R5, R6, R7, R8, R9, R10, R11, R12>(R0, R1, R2, R3, R4, R5, R6, R7, R8, R9, R10, R11, R12) -> some ResolverSpecification

static func buildBlock&lt;R0, R1, R2, R3, R4, R5, R6, R7, R8, R9, R10, R11, R12, R13>(R0, R1, R2, R3, R4, R5, R6, R7, R8, R9, R10, R11, R12, R13) -> some ResolverSpecification

static func buildBlock&lt;R0, R1, R2, R3, R4, R5, R6, R7, R8, R9, R10, R11, R12, R13, R14>(R0, R1, R2, R3, R4, R5, R6, R7, R8, R9, R10, R11, R12, R13, R14) -> some ResolverSpecification

static func buildExpression&lt;ResolverType>(ResolverType) -> ResolverType

static func buildPartialBlock&lt;each Accumulated, R>(accumulated: ResolverSpecificationBuilder&lt;Property>.Specification&lt;Property, repeat each Accumulated>, next: R) -> ResolverSpecificationBuilder&lt;Property>.Specification&lt;Property, repeat each Accumulated, R>

static func buildPartialBlock&lt;R>(first: R) -> ResolverSpecificationBuilder&lt;Property>.Specification&lt;Property, R>

## See Also

### Managing the resolution process

protocol ResolverSpecification

An internal type that a resolver uses to convert data values.

struct EmptyResolverSpecification

struct StringSearchCriteriaFromStringResolverSpecificification

An internal type that a resolver uses to convert data values.

