

- Natural Language
- NLContextualEmbedding
-  init(language:) 

Initializer

# init(language:)

Creates a contextual embedding from a language.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init?(language: NLLanguage)
```

## Parameters 

`language`  

The language the framework uses to find the most recent embedding suitable for the value you specify.

## See Also

### Creating a contextual embedding

convenience init?(modelIdentifier: String)

Creates a contextual embedding from a model identifier.

init?(script: NLScript)

Creates a contextual embedding from a script.

