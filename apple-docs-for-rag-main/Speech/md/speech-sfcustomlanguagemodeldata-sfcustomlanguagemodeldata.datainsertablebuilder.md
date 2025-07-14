

- Speech
- SFCustomLanguageModelData
-  SFCustomLanguageModelData.DataInsertableBuilder 

Structure

# SFCustomLanguageModelData.DataInsertableBuilder

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.1+watchOS 10.0+

``` source
@resultBuilder
struct DataInsertableBuilder
```

## Topics

### Type Methods

static func buildArray([any DataInsertable]) -> any DataInsertable

static func buildBlock(any DataInsertable...) -> any DataInsertable

static func buildEither(first: any DataInsertable) -> any DataInsertable

static func buildEither(second: any DataInsertable) -> any DataInsertable

static func buildOptional((any DataInsertable)?) -> any DataInsertable

## See Also

### Structures

struct CompoundTemplate

struct CustomPronunciation

struct PhraseCount

struct PhraseCountsFromTemplates

struct TemplateInsertableBuilder

