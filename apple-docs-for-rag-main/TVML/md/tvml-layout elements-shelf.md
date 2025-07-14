

- TVML
- Layout Elements
-  shelf 

# shelf

Displays elements horizontally and adds the ability to scroll to offscreen elements.

## Overview

The `shelf` element is a horizontal row consisting of one or more elements. The user navigates along the items on a shelf by clicking left or right on the remote, and chooses an element by clicking the Select button on the remote. The generic shelf element structure is displayed first, followed by several standard shelf configurations. Here’s an example showing the basic layout of a `shelf` element.

```

        Viewers Also Watched

         //add link to other prodcut on your server here

                 //add link to preview image for other product

            Also Watched One

```

There are several standard shelf configurations that are used to display related content.

### Also-Watched Shelf

The `shelf` element can display information about other products that have been watched by people who have also watched the selected product. The shelf displays the image you associate with the also-watched product, and the title is only displayed when the also-watched product is in focus. Here’s an example of a `shelf` element that contains three other products.

```

        Viewers Also Watched

            Turn

            Road

            Helicopter

```

### Cast-and-Crew Shelf

The `shelf` element can display information about the cast and crew associated with the product. Each person is represented by a large circle that contains the individual’s initials. Below the circle is the individual’s name and the name of the character they play. Here’s an example of a `shelf` element that contains three cast members.

```

        Cast and Crew

            Anne Johnson
            Actor

            Tom Clark
            Actor

            Maria Ruiz
            Actor

```

### Extras Shelf

The `shelf` element can display information about additional items included with the product. Common additional items include deleted scenes, extended scenes, and trailers. The listing below shows an example of a `shelf` element that contains a link to the online extras, a brief description of the extras, and a product trailer.

The extras shelf typically contains two sections. The first section contains an image of the additional items and a description of the items. Users can click the image to access the additional items. The second section contains a preview image of a trailer for the original product that users can click to view the trailer. Additional trailers require additional sections.

```

            Product Extras

             //add link to preview image for extras
            Extras
            Enter text describing the item here
            Add text that talks about anything special included with this item or special requirements needed

            Trailers

         //add link to trailer on your server here

                 //add link to preview image for trailer

            Theatrical Trailer 2m

```

### Review-and-Ratings Shelf

The `shelf` element can display a list of ratings and reviews of the item it is associated with. Typically, a `lockup` element is displayed, followed by one or more `buttonLockup` elements. Common rating lockups contain information from iTunes or Rotten Tomatoes.

```

      Reviews and Ratings

         4.1 / 5

         Average of 2,241 iTunes user ratings and reviews.

          99%
         Tomatometer

                  175

               Reviews

                  173

               Fresh

                  2

               Rotten

         WWDC Review
         Brief review here
         Ravi Patel June, 8 2015

```

### Subelements of shelf

- header

- section

- text

### Elements that Use shelf

- alertTemplate

- descriptiveAlertTemplate

- footer

- productBundleTemplate

- productTemplate

- separator

## Topics

### Valid TVML Styles

margin

Specifies the spacing around an element.

padding

Specifies the padding between the border and contents of an element.

tv-interitem-spacing

Specifies the spacing between child elements.

### Valid TVML Attributes

autoHighlight

Specifies that the element should initially be in focus.

binding

Associates information in a data item with an element.

centered

Centers media items in a shelf.

itemID

Mark elements for reuse during DOM updates.

needsMoreThreshold

Sets the amount of remaining screen lengths before firing the needs more event.

prototype

Associates a data item type with an element.

rowCount

Specifies the number of rows in a shelf.

theme

Sets the color scheme for an element.

## See Also

### Container Elements

carousel

Arranges images in a row.

grid

Arranges elements in a grid pattern.

imgDeck

Contains several images to be displayed at a later time.

infoTable

Displays contained element information in a vertical format, with each successive element directly below the previous element.

organizer

Creates a generic element with its contained elements arranged through TVML styles.

row

Displays elements horizontally.

section

Combines elements and acts as a single element.

stack

Groups and lays out elements vertically.

