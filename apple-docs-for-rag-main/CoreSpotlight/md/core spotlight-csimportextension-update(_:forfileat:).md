

- Core Spotlight
- CSImportExtension
-  update(\_:forFileAt:) 

Instance Method

# update(\_:forFileAt:)

Provides searchable attributes for a file at the specified URL.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
func update(
    _ attributes: CSSearchableItemAttributeSet,
    forFileAt contentURL: URL
) throws
```

## Parameters 

`attributes`  

The attribute set for the file at `contentURL`.

`contentURL`  

The URL of the file to provide attributes for.

## Discussion

When Core Spotlight invokes this method, update the properties of the attribute set according to the content in the specified file. For a complete list of properties available, see CSSearchableItemAttributeSet.

Important

Core Spotlight indexes files in batches and may call this method simultaneously on multiple queues with different values of `contentURL`.

