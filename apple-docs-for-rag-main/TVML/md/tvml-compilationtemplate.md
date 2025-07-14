

- TVML
-  compilationTemplate 

# compilationTemplate

Displays information about a single media item and its components.

## Overview

Use the `compilationTemplate` element to display information about one product that is made up of several distinct pieces; for example, an album and all of the songs that it contains. The header area on the left side of the screen contains general product information. Directly underneath the header area are several section areas that group like types of information; for example, one section can contain all of the songs on the album. The related content on the right side of the screen contains any images associated with the product and buttons that the user can use to interact with the product, such as Play and Buy buttons. The following figure shows the basic layout for a `compilationTemplate` page. The theme for the compilation template defaults to the system preference.

### Main Elements

The following listing shows the main elements of the `compilationTemplate` element in TVML format:

```

        …

                …

            …

                Title

                …

```

#### Element Descriptions

background  
Background elements, such as audio.

header  
Information describing what a section of the list contains.

itemBanner  
Product information and row elements, such as button information, that are displayed along the right side of the screen.

list  
Element containing all the content in the template (except background).

listItemLockup  
Elements containing elements used to create one item in a list.

relatedContent  
Element containing all elements displayed along the right side of the screen.

section  
An area of the page that groups related elements for layout purposes.

### Example

The following listing shows the TVML for a `compilationTemplate` example. The example displays a list on the left side that contains information about the album and a list of available songs. The right side of the display contains an image of the album and buttons prompting the user to buy, rate, or shuffle the music.

```

                            Add

                            Rate

                            Shuffle

                WWDC Roadtrip Soundtrack
                Various Artists

                    Instrumental
                    5 Songs
                    2015

                Songs from your favorite movie

                    1
                    Opening sequence
                    11:14

                    2
                    Fight song
                    3:47

                    3
                    Love theme
                    6:48

                    4
                    Car chase
                    5:21

                    5
                    End credit theme
                    8:03

```

The following figure shows the output for the above example:

## Topics

### Valid TVML Attributes

autoHighlight

Specifies that the element should initially be in focus.

binding

Associates information in a data item with an element.

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

productTemplate

Displays detailed information about a single product.

ratingTemplate

Displays a rating for an item.

searchTemplate

Searches for a media item based on user input.

