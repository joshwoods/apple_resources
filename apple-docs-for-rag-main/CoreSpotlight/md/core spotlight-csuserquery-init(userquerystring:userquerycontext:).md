

- Core Spotlight
- CSUserQuery
-  init(userQueryString:userQueryContext:) 

Initializer

# init(userQueryString:userQueryContext:)

Creates a new user query that searches for the specified term.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
init(
    userQueryString: String?,
    userQueryContext: CSUserQueryContext?
)
```

## Parameters 

`userQueryString`  

The term to search for. You may specify an empty string for this parameter.

`userQueryContext`  

A context object with options for how to run the query and generate results.

## Return Value

An initialized query object.

