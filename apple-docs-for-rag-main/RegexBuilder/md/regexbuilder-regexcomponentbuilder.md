

- RegexBuilder
-  RegexComponentBuilder 

Enumeration

# RegexComponentBuilder

A custom parameter attribute that constructs regular expressions from closures.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
@resultBuilder
enum RegexComponentBuilder
```

## Overview

You typically see `RegexComponentBuilder` as a parameter attribute for `Regex`- or `RegexComponent`-producing closure parameters, allowing those closures to combine multiple regular expression components. Type initializers and string algorithm methods in the RegexBuilder framework include a builder closure parameter, so that you can use regular expression components together.

## Topics

### Type Methods

static func buildBlock() -> Regex&lt;Substring>

static func buildExpression&lt;R>(R) -> R

static func buildLimitedAvailability&lt;W, C1, C2>(some RegexComponent) -> Regex&lt;(Substring, C1?, C2?)>

static func buildLimitedAvailability&lt;W, C1, C2, C3, C4, C5, C6, C7, C8>(some RegexComponent) -> Regex&lt;(Substring, C1?, C2?, C3?, C4?, C5?, C6?, C7?, C8?)>

static func buildLimitedAvailability&lt;W, C1, C2, C3, C4, C5, C6>(some RegexComponent) -> Regex&lt;(Substring, C1?, C2?, C3?, C4?, C5?, C6?)>

static func buildLimitedAvailability&lt;W, C1, C2, C3, C4, C5, C6, C7>(some RegexComponent) -> Regex&lt;(Substring, C1?, C2?, C3?, C4?, C5?, C6?, C7?)>

static func buildLimitedAvailability&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9>(some RegexComponent) -> Regex&lt;(Substring, C1?, C2?, C3?, C4?, C5?, C6?, C7?, C8?, C9?)>

static func buildLimitedAvailability&lt;W, C1, C2, C3>(some RegexComponent) -> Regex&lt;(Substring, C1?, C2?, C3?)>

static func buildLimitedAvailability&lt;W, C1, C2, C3, C4>(some RegexComponent) -> Regex&lt;(Substring, C1?, C2?, C3?, C4?)>

static func buildLimitedAvailability&lt;W, C1>(some RegexComponent) -> Regex&lt;(Substring, C1?)>

static func buildLimitedAvailability&lt;W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(some RegexComponent) -> Regex&lt;(Substring, C1?, C2?, C3?, C4?, C5?, C6?, C7?, C8?, C9?, C10?)>

static func buildLimitedAvailability(some RegexComponent) -> Regex&lt;Substring>

static func buildLimitedAvailability&lt;W, C1, C2, C3, C4, C5>(some RegexComponent) -> Regex&lt;(Substring, C1?, C2?, C3?, C4?, C5?)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5)>

static func buildPartialBlock&lt;W0>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;Substring>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8)>

static func buildPartialBlock&lt;W0, W1, C1, C2>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10)>

static func buildPartialBlock&lt;W0, C0, C1, C2, C3, C4, C5>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C0, C1, C2, C3, C4, C5)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6)>

static func buildPartialBlock&lt;W0, C0, C1, C2, C3, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C0, C1, C2, C3, C4, C5, C6, C7, C8, C9)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4)>

static func buildPartialBlock&lt;W0, C0, C1>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C0, C1)>

static func buildPartialBlock&lt;W0, C0, C1, C2>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C0, C1, C2)>

static func buildPartialBlock&lt;W0, W1, C1>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1)>

static func buildPartialBlock&lt;W0, C0>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C0)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3)>

static func buildPartialBlock&lt;W0, C0, C1, C2, C3>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C0, C1, C2, C3)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7)>

static func buildPartialBlock&lt;W0, C0, C1, C2, C3, C4>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C0, C1, C2, C3, C4)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8)>

static func buildPartialBlock&lt;W0, C0, C1, C2, C3, C4, C5, C6>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C0, C1, C2, C3, C4, C5, C6)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10)>

static func buildPartialBlock&lt;W0, W1, C1, C2>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6)>

static func buildPartialBlock&lt;W0, C0, C1, C2, C3, C4, C5, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C0, C1, C2, C3, C4, C5, C6, C7)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3)>

static func buildPartialBlock&lt;W0, C0, C1, C2, C3, C4, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C0, C1, C2, C3, C4, C5, C6, C7, C8)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8)>

static func buildPartialBlock&lt;W0, W1, C1, C2, C3, C4, C5, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> Regex&lt;(Substring, C1, C2, C3, C4, C5, C6, C7)>

static func buildPartialBlock&lt;R>(first: R) -> Regex&lt;R.RegexOutput>

## See Also

### Builders

struct AlternationBuilder

A custom parameter attribute that constructs regular expression alternations from closures.

