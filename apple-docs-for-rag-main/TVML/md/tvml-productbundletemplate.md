

- TVML
-  productBundleTemplate 

# productBundleTemplate

Displays information for a group of related media items.

## Overview

Use the `productBundleTemplate` element to display detailed information about a product bundle, such as a page that describes a television series, including information about the actors, ratings, and series episodes. The top two-thirds of the screen displays general information about the product. The shelf at the bottom provides a row of related items, such as episodes of the show. A user can scroll down and access detailed information about the product, such as critical reviews, actor biographies, and information about any included extras.

The default theme for a product bundle template is `dark` when you specify a background image; otherwise, the product bundle template defaults to the system preference. You can also change the look of a `productBundleTemplate` page by removing `heroImage` from the `stack` element and replacing it with an `img` element that covers the entire screen.

The following figure shows the basic layout for a `productBundleTemplate` page.

### Main Elements

The following listing shows the main elements of the `productBundleTemplate` element in TVML format.

```

                …

                …
                …

        !— Everything following is under the fold —>

            …

```

#### Element Descriptions

background  
Images or audio to be presented in the background.

banner  
Element containing various elements that provide primary information about the product, such as a TV show title and episode title, description, and buttons for purchasing or previewing.

buttonLockup  
A type of button that can contain an image (the `badge` element) as well as text.

description  
The text that describes the show.

heroImg  
An image of the show.

productInfo  
Technical information about the product bundle, such as a show’s runtime, language availability, and accessibility information.

row  
A group of information elements.

shelf  
An element containing row elements. Several shelves are used to display information like shows other users have watched and extra features provided by this product.

stack  
Basic information about the product, including the title, rating, and a description.

subtitle  
Text that provides additional information about its containing element.

text  
The text used to describe the surrounding elements.

title  
The title describing its containing element.

### Example

The following listing shows the TVML for a `productBundleTemplate` example.

```

                WWDC Road Trip

                     99%
                    1hr 54min
                    Comedy
                    2015

                Follow the adventures of a determined developer
                The story of a development team that loves to cook and makes an app for ordering soup. Follow their journey across the country to WWDC, and the meals they make along the way.

                        Preview

                        $9.99
                        Buy

                3 Episodes

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

                    Subtitles for the deaf and Hard of Hearing (SDH) refer to subtitles in the original language with the addition of relevant non-dialog information.

```

The following figures show the two pages created using the above example. The first figure shows what appears immediately onscreen, while the second figure shows what the user sees after navigating down the screen.

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

productTemplate

Displays detailed information about a single product.

ratingTemplate

Displays a rating for an item.

searchTemplate

Searches for a media item based on user input.

