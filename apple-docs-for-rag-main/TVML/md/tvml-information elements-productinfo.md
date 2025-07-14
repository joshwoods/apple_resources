

- TVML
- Information Elements
-  productInfo 

# productInfo

Contains general information about a product.

## Overview

The `productInfo` element contains all of the elements required to describe a product. It commonly contains such information as a product’s title, type, format, running time, and so on. Here’s an example that describes a video, including its run time and languages.

```

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

### Subelements of productInfo

- header

- infoTable

- row

- text

### Elements that Use productInfo

- productBundleTemplate

- productTemplate

## Topics

### Valid TVML Styles

padding

Specifies the padding between the border and contents of an element.

tv-interitem-spacing

Specifies the spacing between child elements.

### Valid TVML Attributes

binding

Associates information in a data item with an element.

prototype

Associates a data item type with an element.

theme

Sets the color scheme for an element.

## See Also

### General Information Elements

info

Displays grouped sets of information.

