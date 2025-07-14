

- Core Spotlight
-  CSUserQuery 

Class

# CSUserQuery

A type you use to initiate searches from your interface and offer suggested text completions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class CSUserQuery
```

## Mentioned in 

Building a search interface for your app

## Overview

A `CSUserQuery` object provides the back-end support for your app’s search features. Combine this object with your app’s search interface to perform lexical and semantic searches of human-entered search terms. You can configure a query object to return ranked or unranked results. You can also use it to get a list of suggestions to display from your search interface.

When the text in your search control changes, create a query object to begin searching for results based on the current text. You use a query object only once to perform a search. If the text changes again while you a previous query is in progress, cancel the old query and execute the new one. For this reason, it’s a good idea to delay the start of each query until there is a sufficient gap between changes.

Configure the query parameters using a CSUserQueryContext object, which you can reuse for multiple queries. The context lets you configure the behavior for ranking results, specify the maximum number of results and suggestions, and filter the results using a predicate string. When you’re ready to start the query, choose one of the following options:

- Get the value of the responses property and iterate over the results.

- Configure the foundItemsHandler property and call start() to execute the query manually.

Each query runs until Spotlight returns the requested maximum number of results. If you don’t specify the maximum number of results, Spotlight runs until it returns all results. To end a search before you receive all the results, call the cancel() method. Cancelling a query is especially important if you’re about to start a new query with an updated search string.

For more information about configuring a `CSUserQuery` object, see Building a search interface for your app.

## Topics

### Creating a user query

init(userQueryString: String?, userQueryContext: CSUserQueryContext?)

Creates a new user query that searches for the specified term.

### Preparing to search

class func prepare()

Performs one-time tasks that prepare Spotlight to search for content in all search indexes.

class func prepareProtectionClasses([FileProtectionType])

Performs one-time tasks that prepare Spotlight to search for content in one or more protected search indexes.

### Executing the query automatically

var responses: CSUserQuery.Responses

The matching results and suggestions for the current query string.

var suggestions: CSUserQuery.Suggestions

An asynchronous sequence of suggested completions for the current query text.

struct Responses

An asynchronous sequence that contains the results and suggestions for a query string.

struct Suggestions

An asynchronous sequence that contains the suggested completions for a search string.

struct Item

A search result that the query returns in a response.

struct Suggestion

A suggested text completion for a query’s search term.

### Executing the query with handler blocks

func start()

Starts searching the index for items that match the current query string and parameters.

func cancel()

Cancels the current query operation.

var foundSuggestionsHandler: (([CSSuggestion]) -> Void)?

The block to execute when the query delivers a new batch of suggested items.

var foundSuggestionCount: Int

The number of suggested items the query found so far.

### Improving the quality of ranked results

func userEngaged(CSUserQuery.Item, visibleItems: [CSUserQuery.Item], interaction: CSUserQuery.UserInteractionKind)

Notifies the system that someone engaged with a specific search result in your app’s interface.

func userEngaged(CSUserQuery.Suggestion, visibleSuggestions: [CSUserQuery.Suggestion], interaction: CSUserQuery.UserInteractionKind)

Notifies the system that someone engaged with a specific text completion in your app’s interface.

enum UserInteractionKind

Constants that indicate how someone engaged with search-related content.

## Relationships

### Inherits From

- CSSearchQuery

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Queries

Building a search interface for your app

Add a search interface to your app to execute Spotlight queries and offer suggested text completions.

Searching for information in your app

Search for app-specific content and refine search results using predicates and filters.

class CSUserQueryContext

The configuration details to apply to a user query.

class CSSearchQuery

A type you use to programmatically search the indexed app content.

class CSSearchQueryContext

The behavior configuration to use for a search query.

class CSSuggestion

The kind of suggestion to use in a query.

