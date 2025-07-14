

- Core Spotlight
- CSUserQueryContext
-  init(currentSuggestion:) 

Initializer

# init(currentSuggestion:)

Creates a new query context object with an optional suggested search string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
init(currentSuggestion: CSSuggestion?)
```

## Parameters 

`currentSuggestion`  

The suggested text completion that the person selected in your interface. Specify `nil` if the person hasn’t chosen a suggestion.

## Return Value

An initialized user query context object. Configure the properties of the returned object and use it to construct a CSUserQuery object.

