

- Media Player
- MPMediaPropertyPredicate
-  init(value:forProperty:) 

Initializer

# init(value:forProperty:)

Creates a media property predicate with the default comparison type.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
init(
    value: Any?,
    forProperty property: String
)
```

## Parameters 

`value`  

The property value that you want to match when you query the Music library. For example, if you specify the MPMediaItemPropertyArtist constant in the `forProperty` parameter, in this parameter you supply a string containing the artist name.

`property`  

A property to use to build a media property predicate. See Media item types and keys.

## Return Value

A media property predicate.

## Discussion

This is a convenience method that uses the default logical comparison type of MPMediaPredicateComparison.equalTo.

## See Also

### Creating media property predicates

init(value: Any?, forProperty: String, comparisonType: MPMediaPredicateComparison)

Creates a media property predicate with a specified comparison type.

