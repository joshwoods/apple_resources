

- Media Player
- MPMediaPropertyPredicate
-  init(value:forProperty:comparisonType:) 

Initializer

# init(value:forProperty:comparisonType:)

Creates a media property predicate with a specified comparison type.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
init(
    value: Any?,
    forProperty property: String,
    comparisonType: MPMediaPredicateComparison
)
```

## Parameters 

`value`  

The property value that you want to match when you query the Music library. For example, if you specify the `MPMediaItemPropertyArtist` constant in the `forProperty` parameter, in this parameter you supply a string containing the artist name.

`property`  

A property to use to build a media property predicate. See General Media Item Property Keys and Podcast Item Property Keys in MPMediaItem.

`comparisonType`  

: The logical comparison type for the predicate. See MPMediaPredicateComparison.

## Return Value

A media property predicate.

## See Also

### Creating media property predicates

init(value: Any?, forProperty: String)

Creates a media property predicate with the default comparison type.

