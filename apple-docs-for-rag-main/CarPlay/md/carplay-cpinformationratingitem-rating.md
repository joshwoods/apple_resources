

- CarPlay
- CPInformationRatingItem
-  rating 

Instance Property

# rating

The current rating that the template displays.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var rating: NSNumber? { get }
```

## Discussion

This property is an NSNumber that contains a value in the range of 0 to maximumRating. The value is an increment of 0.5.

## See Also

### Accessing the Item’s Attributes

var maximumRating: NSNumber?

The maximum rating that the template displays.

