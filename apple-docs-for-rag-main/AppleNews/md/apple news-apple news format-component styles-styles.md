

- Apple News
- Apple News Format
-  Component Styles 

API Collection

# Component Styles

Learn to use component styles to add borders, set background colors, and apply background images to components and to set the styling for tables.

## Overview

Component styles are at the heart of creating a unique article with Apple News Format. They provide options that range from adding background images and drawing borders to setting the styles for the rows, columns, and cells in a table.

## Topics

### Component Style Basics

Defining a Component Style

Set style options for the components in your article.

object ComponentStyle

The object for setting style properties for components, including background color and fill, borders, and table styles.

object CornerMask

The object for creating rounded corners.

object Border

The object for setting borders for component sides or tables.

object StrokeStyle

The object for defining the color, width, and style of a border or divider.

### Backgrounds for Components

Applying a Background to a Component

Change the appearance of the backgrounds in your article.

object ImageFill

The object for adding an image background fill to a component.

object RepeatableImageFill

The object for adding a background image that Apple News can repeat.

object VideoFill

The object for adding a video background fill to a component.

object LinearGradientFill

The object for displaying a linear gradient as a component background.

object GradientFill

The properties all gradient fill types share.

object Fill

The object for setting a fill type and attachment for a component’s background fill.

object ColorStop

The object for specifying the color and location for a color stop in a gradient.

### Component Effects

object ComponentShadow

The object for creating a component shadow.

object ComponentShadowOffset

The object for setting an offset value to use with a component shadow.

### Table Styles

Defining and Using Table Styles

Apply table styles, such as borders and backgrounds, to the rows, columns, and cells in your HTML and JSON tables.

object TableStyle

The object for defining a style for rows, columns, cells, and headers in a table.

object TableRowStyle

The object for applying styles to rows in a table.

object ConditionalTableRowStyle

The object for applying styles to table rows that meet certain conditions.

object TableRowSelector

The object for defining conditions that apply a conditional style to a row.

object TableColumnStyle

The object for applying styles to columns in a table.

object ConditionalTableColumnStyle

The object for applying styles to table columns that meet certain conditions.

object TableColumnSelector

The object for defining conditions that apply a conditional style to a column.

object TableCellStyle

The object for applying styles to cells in a table.

object ConditionalTableCellStyle

The object for applying a style to table cells that meet certain conditions.

object TableCellSelector

The object for defining conditions that apply a conditional style to a cell.

object TableBorder

The object for setting borders for tables.

object TableStrokeStyle

The object for defining the color, width, and style of a stroke in a table.

object Padding

The object for defining space around the content in a table cell.

object FormattedText

The object for specifying formatted text content and styling for captions in table cells.

## See Also

### Related Documentation

Apple News Format Tutorials

Create a basic article and then add advanced design features.

### Styles

Enhancing Your Articles with Styles

Improve the appearance of the text and components in your article by using Apple News Format styles.

Supporting Dark Mode for Your Article

Update your article template so that your article adapts when Dark Mode is active.

object DocumentStyle

The object for setting the background color for your article.

Text Styles

Learn about text styles and how to apply them to your text and text components.

Supported Color Names

Learn the color names supported in Apple News Format.

type Color

The strings for defining colors in Apple News Format.

