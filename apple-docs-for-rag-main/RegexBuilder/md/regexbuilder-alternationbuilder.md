

- RegexBuilder
-  AlternationBuilder 

Structure

# AlternationBuilder

A custom parameter attribute that constructs regular expression alternations from closures.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
@resultBuilder
struct AlternationBuilder
```

## Overview

When you use a `ChoiceOf` initializer, the initializer’s closure parameter has an `AlternationBuilder` attribute, allowing you to provide multiple regular expression statements as alternatives.

## Topics

### Type Methods

static func buildExpression&lt;R>(R) -> R

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, W1, C5, C6>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5?, C6?)>

static func buildPartialBlock&lt;W0, C1, W1, C2>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, W1, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6?, C7?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8)>

static func buildPartialBlock&lt;W0, C1, C2, C3>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, C6, C7, C8, C9, W1, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10?)>

static func buildPartialBlock&lt;W1, C1, C2, C3, C4, C5>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1?, C2?, C3?, C4?, C5?)>

static func buildPartialBlock&lt;W0, C1, W1, C2, C3, C4, C5, C6>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2?, C3?, C4?, C5?, C6?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, W1, C5, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5?, C6?, C7?)>

static func buildPartialBlock&lt;W1, C1, C2, C3, C4>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1?, C2?, C3?, C4?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6, C7)>

static func buildPartialBlock&lt;W1, C1, C2, C3, C4, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1?, C2?, C3?, C4?, C5?, C6?, C7?, C8?)>

static func buildPartialBlock&lt;W0, C1, C2, W1, C3, C4, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3?, C4?, C5?, C6?, C7?, C8?, C9?, C10?)>

static func buildPartialBlock&lt;W0, C1, W1, C2, C3, C4>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2?, C3?, C4?)>

static func buildPartialBlock&lt;W0, C1, C2, W1, C3, C4, C5, C6>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3?, C4?, C5?, C6?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, W1, C5>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, W1, C4, C5>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4?, C5?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, C6, C7, W1, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8?, C9?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, W1, C4, C5, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4?, C5?, C6?, C7?)>

static func buildPartialBlock&lt;W0, C1, C2, W1, C3, C4, C5, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3?, C4?, C5?, C6?, C7?)>

static func buildPartialBlock&lt;W0, C1>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1)>

static func buildPartialBlock(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;Substring>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, W1, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5?, C6?, C7?, C8?, C9?, C10?)>

static func buildPartialBlock&lt;W0, C1, C2, W1, C3, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3?, C4?, C5?, C6?, C7?, C8?, C9?)>

static func buildPartialBlock&lt;W0, C1, W1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2?, C3?, C4?, C5?, C6?, C7?, C8?, C9?, C10?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, C6>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, W1, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6?, C7?, C8?, C9?, C10?)>

static func buildPartialBlock&lt;W0, C1, C2, W1, C3, C4>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3?, C4?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, C6, W1, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6, C7?, C8?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, C6, C7, W1, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8?, C9?, C10?)>

static func buildPartialBlock&lt;W1, C1, C2, C3>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1?, C2?, C3?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, W1, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6?, C7?, C8?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5)>

static func buildPartialBlock&lt;W0, C1, C2, C3, W1, C4>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, W1, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4?, C5?, C6?, C7?, C8?, C9?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, W1, C4, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4?, C5?, C6?, C7?, C8?)>

static func buildPartialBlock&lt;W0, C1, W1, C2, C3>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2?, C3?)>

static func buildPartialBlock&lt;W1, C1>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9)>

static func buildPartialBlock&lt;W0, C1, C2, W1, C3, C4, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3?, C4?, C5?, C6?, C7?, C8?)>

static func buildPartialBlock&lt;W1, C1, C2>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1?, C2?)>

static func buildPartialBlock&lt;W1, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1?, C2?, C3?, C4?, C5?, C6?, C7?, C8?, C9?, C10?)>

static func buildPartialBlock&lt;W0, C1, C2, W1, C3>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, W1, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5?, C6?, C7?, C8?, C9?)>

static func buildPartialBlock&lt;W1, C1, C2, C3, C4, C5, C6>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1?, C2?, C3?, C4?, C5?, C6?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, C6, C7, C8, W1, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, W1, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6?, C7?, C8?, C9?)>

static func buildPartialBlock&lt;W0, C1, W1, C2, C3, C4, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2?, C3?, C4?, C5?, C6?, C7?, C8?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, W1, C4, C5, C6, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4?, C5?, C6?, C7?, C8?, C9?, C10?)>

static func buildPartialBlock&lt;W0, C1, C2>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2)>

static func buildPartialBlock&lt;W0, C1, C2, C3, W1, C4, C5, C6>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4?, C5?, C6?)>

static func buildPartialBlock&lt;W0, C1, W1, C2, C3, C4, C5, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2?, C3?, C4?, C5?, C6?, C7?)>

static func buildPartialBlock&lt;W0, C1, W1, C2, C3, C4, C5>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2?, C3?, C4?, C5?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, W1, C6>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, C6, W1, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6, C7?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, C6, W1, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6, C7?, C8?, C9?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, W1, C5, C6, C7, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5?, C6?, C7?, C8?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, C6, C7, W1, C8>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8?)>

static func buildPartialBlock&lt;W0, C1, C2, W1, C3, C4, C5>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3?, C4?, C5?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, C6, W1, C7, C8, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6, C7?, C8?, C9?, C10?)>

static func buildPartialBlock&lt;W1, C1, C2, C3, C4, C5, C6, C7>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1?, C2?, C3?, C4?, C5?, C6?, C7?)>

static func buildPartialBlock&lt;W0, C1, C2, C3, C4, C5, C6, C7, C8, W1, C9, C10>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2, C3, C4, C5, C6, C7, C8, C9?, C10?)>

static func buildPartialBlock&lt;W1, C1, C2, C3, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1?, C2?, C3?, C4?, C5?, C6?, C7?, C8?, C9?)>

static func buildPartialBlock&lt;W0, C1, W1, C2, C3, C4, C5, C6, C7, C8, C9>(accumulated: some RegexComponent, next: some RegexComponent) -> ChoiceOf&lt;(Substring, C1, C2?, C3?, C4?, C5?, C6?, C7?, C8?, C9?)>

static func buildPartialBlock&lt;R, W, C1, C2>(first: R) -> ChoiceOf&lt;(W, C1?, C2?)>

static func buildPartialBlock&lt;R, W, C1, C2, C3, C4, C5, C6>(first: R) -> ChoiceOf&lt;(W, C1?, C2?, C3?, C4?, C5?, C6?)>

static func buildPartialBlock&lt;R, W, C1, C2, C3, C4, C5>(first: R) -> ChoiceOf&lt;(W, C1?, C2?, C3?, C4?, C5?)>

static func buildPartialBlock&lt;R, W, C1>(first: R) -> ChoiceOf&lt;(W, C1?)>

static func buildPartialBlock&lt;R, W, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10>(first: R) -> ChoiceOf&lt;(W, C1?, C2?, C3?, C4?, C5?, C6?, C7?, C8?, C9?, C10?)>

static func buildPartialBlock&lt;R, W, C1, C2, C3, C4, C5, C6, C7>(first: R) -> ChoiceOf&lt;(W, C1?, C2?, C3?, C4?, C5?, C6?, C7?)>

static func buildPartialBlock&lt;R, W, C1, C2, C3, C4>(first: R) -> ChoiceOf&lt;(W, C1?, C2?, C3?, C4?)>

static func buildPartialBlock&lt;R, W, C1, C2, C3, C4, C5, C6, C7, C8, C9>(first: R) -> ChoiceOf&lt;(W, C1?, C2?, C3?, C4?, C5?, C6?, C7?, C8?, C9?)>

static func buildPartialBlock&lt;R>(first: R) -> ChoiceOf&lt;R.RegexOutput>

static func buildPartialBlock&lt;R, W, C1, C2, C3>(first: R) -> ChoiceOf&lt;(W, C1?, C2?, C3?)>

static func buildPartialBlock&lt;R, W, C1, C2, C3, C4, C5, C6, C7, C8>(first: R) -> ChoiceOf&lt;(W, C1?, C2?, C3?, C4?, C5?, C6?, C7?, C8?)>

## See Also

### Builders

enum RegexComponentBuilder

A custom parameter attribute that constructs regular expressions from closures.

