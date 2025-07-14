

- TVML
-  productTemplate 

# productTemplate

Displays detailed information about a single product.

## Overview

Use the `productTemplate` element to display, for example, a page that describes a movie, including information about the actors, ratings, and like movies. The page displays general information about the product in the top two-thirds of the screen with a row of related products directly below. A user can scroll down and access detailed information about the product, including critical reviews, actor biographies, and information about any included extras.

The following figure shows the basic layout for a `productTemplate` page. The default theme for a product template is `dark` when a background image is specified; otherwise, the product template defaults to the system preference.

### Main Elements

The following listing shows the main elements of the productTemplate element in TVML format.

```

            …
            …

            …

```

Note

You can change the look of a `productTemplate` page by removing `heroImage` from the `stack` element and replacing it with an `img` element that covers the entire screen.

#### Element Descriptions

banner  
Element containing subelements that provide primary information about a product, such as a movie title, description, credits, and purchase information.

buttonLockup  
A type of button that can contain an image (the `badge` element) as well as text.

description  
Text that describes the product in detail; for example, a movie synopsis.

heroImg  
An image of the product.

infoList  
Product information such as actors, directors, and producers.

productInfo  
Technical information about the product such as runtime, language availability, and accessibility information.

row  
A group of information elements.

shelf  
An element containing row elements. Several shelves are used to display information like shows other users have watched and extra features provided by this product.

stack  
Basic information about the product, including the title, rating, and a description.

subtitle  
Text that provides additional information about its containing element.

title  
The title describing its containing element.

### Example

The following listing shows the TVML for a `productTemplate` example:

```

                  Director

               John Appleseed

                  Actors

               Anne Johnson
               Tom Clark
               Maria Ruiz

            WWDC Road Trip

                99%
               1hr 54min
               Comedy
               2015

            An aspiring developer gets a ticket to WWDC at the last minute. Now they need to get across country in time for the keynote, and the only person who can help is their quirky roommate.
            Language information can go here

                  Preview

                  $9.99
                  Buy

            Viewers Also Watched

               Turn

               Road

               Helicopter

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

            Cast and Crew

               Anne Johnson
               Actor

               Tom Clark
               Actor

               Maria Ruiz
               Actor

               Information

                  Studio

               Apple

                  Runtime

               1:54

                  Format

               Widescreen

               Languages

                  Primary

               English (Dolby 5.1), Subtitles, CC

                  Additional

               Cantonese (Subtitles)

               Accessibility

                  SDH

               Subtitles for the deaf and Hard of Hearing (SDH) refer to subtitles in the original lanuage with the addition of relevant non-dialog information.

```

The following figures show the ouput for the above example. The first figure shows the output for the example when it first appears on screen. The second figure shows the output below the fold as the user scrolls down the screen.

## Topics

### Valid TVML Attributes

binding

Associates information in a data item with an element.

itemID

Mark elements for reuse during DOM updates.

layoutDirection

Specifies the direction in which text is displayed.

prototype

Associates a data item type with an element.

theme

Sets the color scheme for an element.

## See Also

### Full-Page Templates

alertTemplate

Displays important information to the user.

catalogTemplate

Displays groups of items along one side of a page and images of a group’s contents on the other side.

compilationTemplate

Displays information about a single media item and its components.

descriptiveAlertTemplate

Displays large amounts of important information to the user.

divTemplate

Provides the ability to create pages that don’t conform to a layout defined by another template.

formTemplate

Provides the ability to gather information from the user.

listTemplate

Displays a list of items along one side of a page and the corresponding image on the other side.

loadingTemplate

Displays a spinner and description on the screen.

mainTemplate

Displays user options for a media item.

menuBarTemplate

Creates a page with items along the top and related information below.

oneupTemplate

Creates a page that allows users to navigate between full-screen images.

paradeTemplate

Displays a groups of items along one side of a page and scrolling images on the other side.

productBundleTemplate

Displays information for a group of related media items.

ratingTemplate

Displays a rating for an item.

searchTemplate

Searches for a media item based on user input.

