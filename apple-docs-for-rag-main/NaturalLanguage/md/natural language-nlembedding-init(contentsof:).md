

- Natural Language
- NLEmbedding
-  init(contentsOf:) 

Initializer

# init(contentsOf:)

Creates a word embedding from a model file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
convenience init(contentsOf url: URL) throws
```

## Parameters 

`url`  

The location of the .`mlmodel` file that contains a word embedding.

## Discussion

Use this initializer to create a word embedding from an `.mlmodel` file saved by Create ML’s MLWordEmbedding.

## See Also

### Creating a word embedding

class func wordEmbedding(for: NLLanguage) -> NLEmbedding?

Retrieves a word embedding for a given language.

class func wordEmbedding(for: NLLanguage, revision: Int) -> NLEmbedding?

Retrieves a word embedding for a given language and revision.

