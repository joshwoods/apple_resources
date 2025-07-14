

- Core Media
-  CMTextMarkup 

API Collection

# CMTextMarkup

Attributes that specify text markup in legible media.

## Overview

Core Media supports legible media streams like subtitles and closed captions. In some cases, apps may need to specify style information to control rendering. In other cases, the framework indicates the text and styling to apply.

## Topics

### Fonts

let kCMTextMarkupAttribute_FontFamilyName: CFString

A name of a font family.

let kCMTextMarkupAttribute_GenericFontFamilyName: CFString

A generic font family name identifier.

let kCMTextMarkupAttribute_BaseFontSizePercentageRelativeToVideoHeight: CFString

A base font size as a percentage of the video height.

let kCMTextMarkupAttribute_RelativeFontSize: CFString

A font size as a percentage of the current default font size.

### Styles

let kCMTextMarkupAttribute_BoldStyle: CFString

A bold font style.

let kCMTextMarkupAttribute_ItalicStyle: CFString

An italic font style.

let kCMTextMarkupAttribute_UnderlineStyle: CFString

An underline font style.

let kCMTextMarkupAttribute_CharacterEdgeStyle: CFString

A style for character edges.

### Colors

let kCMTextMarkupAttribute_ForegroundColorARGB: CFString

A foreground color for the text.

let kCMTextMarkupAttribute_BackgroundColorARGB: CFString

A background color for the text.

let kCMTextMarkupAttribute_CharacterBackgroundColorARGB: CFString

A background color for individual text characters.

### Layout

let kCMTextMarkupAttribute_VerticalLayout: CFString

The vertical layout of a text block.

let kCMTextMarkupAttribute_Alignment: CFString

The text alignment in the writing direction of the first line of text.

let kCMTextMarkupAttribute_TextPositionPercentageRelativeToWritingDirection: CFString

The placement of the block of text as a percentage in the writing direction.

let kCMTextMarkupAttribute_OrthogonalLinePositionPercentageRelativeToWritingDirection: CFString

The placement of the first line in a block of text as a percentage in the direction orthogonal to the writing direction.

let kCMTextMarkupAttribute_WritingDirectionSizePercentage: CFString

The width or height as a percentage of the bounding box that contains the text.

