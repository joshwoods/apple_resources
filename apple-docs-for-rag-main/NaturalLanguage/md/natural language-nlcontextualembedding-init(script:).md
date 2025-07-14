

- Natural Language
- NLContextualEmbedding
-  init(script:) 

Initializer

# init(script:)

Creates a contextual embedding from a script.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init?(script: NLScript)
```

## Parameters 

`script`  

The script the framework uses to find the most recent embedding suitable for the value you specify.

## See Also

### Creating a contextual embedding

convenience init?(modelIdentifier: String)

Creates a contextual embedding from a model identifier.

init?(language: NLLanguage)

Creates a contextual embedding from a language.

