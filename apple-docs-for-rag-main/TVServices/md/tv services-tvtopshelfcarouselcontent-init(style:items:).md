

- TV Services
- TVTopShelfCarouselContent
-  init(style:items:) 

Initializer

# init(style:items:)

Creates a content object for displaying items in a carousel style in the top shelf interface.

tvOS 13.0+

``` source
init(
    style: TVTopShelfCarouselContent.Style,
    items: [TVTopShelfCarouselItem]
)
```

## Parameters 

`style`  

The appearance to use for individual items. For a list of possible values, see TVTopShelfCarouselContent.Style.

`items`  

The items to display in the Top Shelf interface. All of the items in the array must have unique identifiers.

## Return Value

A new carousel content object containing the specified items.

