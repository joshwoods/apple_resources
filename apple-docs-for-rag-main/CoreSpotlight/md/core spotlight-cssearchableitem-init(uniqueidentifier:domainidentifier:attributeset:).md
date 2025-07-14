

- Core Spotlight
- CSSearchableItem
-  init(uniqueIdentifier:domainIdentifier:attributeSet:) 

Initializer

# init(uniqueIdentifier:domainIdentifier:attributeSet:)

Returns a searchable item associated with the specified identifier, domain identifier, and attribute set.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
init(
    uniqueIdentifier: String?,
    domainIdentifier: String?,
    attributeSet: CSSearchableItemAttributeSet
)
```

## Parameters 

`uniqueIdentifier`  

The unique identifier for the item. If you specify `NULL`, an identifier is generated automatically.

`domainIdentifier`  

An identifier for a domain, such as an album, that helps you group items together in a way that makes sense.

`attributeSet`  

A set of properties that specify the metadata you want to display about an item in a search result. See CSSearchableItemAttributeSet for the types of properties you can use.

## Return Value

A searchable item that’s associated with the specified identifier, domain identifier, and attribute set.

