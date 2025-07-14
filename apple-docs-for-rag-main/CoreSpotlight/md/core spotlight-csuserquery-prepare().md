

- Core Spotlight
- CSUserQuery
-  prepare() 

Type Method

# prepare()

Performs one-time tasks that prepare Spotlight to search for content in all search indexes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
class func prepare()
```

## Mentioned in 

Building a search interface for your app

## Discussion

Call this method once during your app’s lifecycle to give Spotlight time to load the resources it needs for search. This preparation comes at a cost, so measure your app’s performance and determine an appropriate time to call it. For example, you might call it when you load an interface that includes search features.

You don’t need to call this method more than once during the lifetime of your app, but it’s safe to call the method multiple times.

## See Also

### Preparing to search

class func prepareProtectionClasses([FileProtectionType])

Performs one-time tasks that prepare Spotlight to search for content in one or more protected search indexes.

