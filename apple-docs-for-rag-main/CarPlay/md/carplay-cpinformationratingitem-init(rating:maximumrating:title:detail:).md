

- CarPlay
- CPInformationRatingItem
-  init(rating:maximumRating:title:detail:) 

Initializer

# init(rating:maximumRating:title:detail:)

Creates a rating item with a current and a maximum rating.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(
    rating: NSNumber?,
    maximumRating: NSNumber?,
    title: String?,
    detail: String?
)
```

## Parameters 

`rating`  

A number in the range of 0 to `maximumRating`. The number must be an increment of 0.5.

`maximumRating`  

A whole number in the range of 1 to 5 that specifies the maximum rating that the item allows.

`title`  

The text that the template displays as the item’s title.

`detail`  

The text that the template displays below or beside the title, depending on the template’s layout. See CPInformationTemplateLayout for more information.

