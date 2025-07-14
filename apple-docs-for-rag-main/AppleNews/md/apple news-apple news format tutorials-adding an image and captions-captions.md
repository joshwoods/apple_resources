

- Apple News
- Apple News Format Tutorials
-  Adding an Image and Captions 

Article

# Adding an Image and Captions

Create a photo that extends to both edges of the display, with captions that appear in the article layout and in full-screen view.

## Overview

In Adding a Divider, you created a divider and used a `ComponentLayout` object to extend the divider to the right edge of the display. Here, you’ll do something similar—you’ll use a `ComponentLayout` object to position a photo against both edges of the display.

**On this page, you’ll learn how to:**

- Add a `photo` component to display an image in your article.

- Add two types of captions: one that appears in the article layout and another that appears when the image is in full screen.

- Make the photo bleed to both edges of the display by using the `ignoreDocumentMargin` property with a value of `"true"`.

- Move the photo caption closer to the content above and below it by using smaller values for the `margin` property.

- Create a new default component text style for components with the `caption` role.

### Define Positions for the Photo and Caption

In Positioning Text Components, you created `ComponentLayout` objects and used them to adjust the positions of your text components. Here, you’ll do something similar, creating new `ComponentLayout` objects for photos and captions. To cause the photo to reach the far right and left edges of the display, you’ll use the `ignoreDocumentMargin` property with a value of `true`.

1.  Copy the example code fullBleedLayout and halfMarginBothLayout: Copy This Code.

2.  Paste the code inside the `ArticleDocument.componentLayouts` object in your `article.json` file, after the closing brace (`}`) of the last `ComponentLayout` object and before the closing brace for the whole `componentLayouts` property.

Your code should look like the example code fullBleedLayout and halfMarginBothLayout: Result.

#### fullBleedLayout and halfMarginBothLayout: Copy This Code

```
,
    "fullBleedLayout": {
      "ignoreDocumentMargin": true
    },
    "halfMarginBothLayout": {
      "columnStart": 0,
      "columnSpan": 14,
      "margin": {
        "top": 12,
        "bottom": 12
      }
    }
```

#### fullBleedLayout and halfMarginBothLayout: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "componentLayouts": {
    ...
    "fullBleedLayout": {
      "ignoreDocumentMargin": true
    },
    "halfMarginBothLayout": {
      "columnStart": 0,
      "columnSpan": 14,
      "margin": {
        "top": 12,
        "bottom": 12
      }
    }
  },
  ...
}
```

### Define a Style for Caption Text

In Creating Your First Article, you created default text styles for component types. Here, you’ll do something similar—create a new default text style for `caption` components.

1.  Copy the example code Caption Text Style: Copy This Code.

2.  Paste the code inside the `ArticleDocument.componentTextStyles` object in your `article.json` file, after the closing brace (`}`) of the last text style and before the closing brace for the whole `componentTextStyles` property.

Your code should look like the example code Caption Text Style: Result.

#### Caption Text Style: Copy This Code

```
,
    "default-caption": {
      "fontName": "IowanOldStyle-Italic",
      "fontSize": 12,
      "lineHeight": 16,
      "paragraphSpacingBefore": 12,
      "paragraphSpacingAfter": 12,
      "textColor": "#53585F"
    }
```

#### Caption Text Style: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "componentTextStyles": {
    ...
    "default-caption": {
      "fontName": "IowanOldStyle-Italic",
      "fontSize": 12,
      "lineHeight": 16,
      "paragraphSpacingBefore": 12,
      "paragraphSpacingAfter": 12,
      "textColor": "#53585F"
    }
  }
  ...
}
```

### Add a Photo and Captions in Your Article

A `photo` component in your JSON file represents a photo in your article. The `"caption"` property of the `photo` component represents some text that is seen when the image is in full screen, and a `caption` component represents some text that is visible in the article.

1.  Copy the example code Photo and Captions: Copy This Code.

2.  Paste the code inside the `components` array of your article, after the closing brace and comma (`},`) that end the `byline` component.

Your code should look like the example code Photo and Captions: Result.

After you make this change in your `article.json` file, you can preview your working `article.json` file in News Preview to see the photo and captions.

#### Photo and Captions: Copy This Code

```
    {
      "role": "photo",
      "layout": "fullBleedLayout",
      "caption": "A caption for the photo.",
      "URL": "bundle://header.jpg"
    },
    {
      "role": "caption",
      "layout": "halfMarginBothLayout",
      "text": "ABOVE: A caption for the photo. (Attribution)"
    },
    {
      "role": "divider",
      "layout": "fullMarginBelowLayout",
      "stroke": {
        "width": 1,
        "color": "#D5B327"
      }
    },
```

#### Photo and Captions: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    ...
    {
      "role": "photo",
      "layout": "fullBleedLayout",
      "caption": "A caption for the photo.",
      "URL": "bundle://header.jpg"
    },
    {
      "role": "caption",
      "layout": "halfMarginBothLayout",
      "text": "ABOVE: A caption for the photo. (Attribution)"
    },
    {
      "role": "divider",
      "layout": "fullMarginBelowLayout",
      "stroke": {
        "width": 1,
        "color": "#D5B327"
      }
    },
    ...
  ],
  ...
}
```

### Further Exploration

At any time, you can try changing property values in your `article.json` file and then use News Preview to see how these changes affect the look of your article.

For example, try changing the URL of your article’s `photo` component:

1.  In your `article.json` file, find the `photo` component in the `components` array.

2.  In the `photo` component, find the `URL` property.

3.  Replace the value of the `URL` property, `"bundle://header.jpg"`, with the URL of an image on your website.

4.  Preview your `article.json` file in News Preview.

The `photo` component now displays your image.

### Previous

Adding a Divider

### Next

Adding a Pull Quote

## See Also

### Related Documentation

object Photo

The component for including a photograph.

object Caption

The component for adding caption text.

object CaptionDescriptor

The object you use in image components for displaying captions when the image is full-screen.

object TextStyle

The object for defining the text style, such as font family, size, and color, that you can apply to ranges of text.

object ComponentTextStyle

The object for defining the style for a text component, including spacing, alignment, and drop caps.

object ComponentLayout

The object for defining the positioning for a specific component within the article’s column system.

### Introductory Design Tutorial

Setting Up the Introductory Tutorial

Download the tutorial files, and learn about what you’ll create in the introductory tutorial.

Creating Your First Article

Create an article with text components and component text styles.

Positioning Text Components

Adjust the positions of the text components in your article—for example, place the article body off-center.

Adding a Divider

Create a horizontal, styled divider that extends to the right edge of the display.

Adding a Pull Quote

Break an existing body component into two components, and then insert a pull quote between them.

Adding a Gallery of Images

Display three images as a sequential gallery.

Adding a Mosaic of Images

Display five images as mosaic tiles.

Adding a Tweet

Include a tweet in an article.

Adding a Podcast

Add a link to a podcast that displays the podcast artwork and the podcast show or episode information.

Viewing the Finished Article for the Introductory Design Tutorial

See the full JSON code from this tutorial.

