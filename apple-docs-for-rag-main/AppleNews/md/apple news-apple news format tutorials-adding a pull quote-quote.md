

- Apple News
- Apple News Format Tutorials
-  Adding a Pull Quote 

Article

# Adding a Pull Quote

Break an existing body component into two components, and then insert a pull quote between them.

## Overview

You can use pull quotes to highlight particularly compelling and relevant points. Visually, a pull quote can break up long portions of text, providing relief to the user.

**On this page, you’ll learn how to:**

- Add a pull quote to your article.

- Use style and layout objects to customize a pull quote, including adding hanging punctuation.

Tip

This example uses curly quotes. If you ever want to use straight quotes instead, make sure you “escape” the straight quotes using a backslash (`\`).

### Add a Pull Quote in Your Article

When a pull quote is accompanied by an attribution line, use two separate `pullquote` components. This allows you to use different layouts and different text styles for the quote text and the attribution text.

First, you’ll break an existing `body` component into two components. Then, you’ll insert two `pullquote` components (representing a pull quote and an attribution) between the `body` components.

1.  In your `article.json` file, copy the `body` component whose text begins with `Quis autem vel eum`, including the component’s opening brace (`{`) and closing brace and comma (`},`)

2.  Paste the component after the brace and comma that end the component that you just copied, so that there are two identical `body` components.

3.  In the first of the two `body` components, delete everything in the `text` property value after `blanditiis`. Do not delete the closing quotation mark.

4.  In the second of the two `body` components, delete everything in the `text` property value before `Cras ulticies`. Do not delete the opening quotation mark.

5.  Copy the example code Pull Quote: Copy This Code.

6.  Paste the code between the two components from steps 1 through 4, after the closing brace and comma.

Your code should look like the example code Pull Quote: Result.

After you make these changes in your code, you can preview your working `article.json` file in News Preview to see the pull quote and attribution.

#### Pull Quote: Copy This Code

```
    {
      "role": "pullquote",
      "text": "“QUIA CONSEQUUNTUR MAGNI DOLORES EOS QUI RATIONE VOLUPTATEM SEQUI NESCIUNT.”"
    },
    {
      "role": "pullquote",
      "text": "— ATTRIBUTION"
    },
```

#### Pull Quote: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    ...
    {
      "role": "pullquote",
      "text": "“QUIA CONSEQUUNTUR MAGNI DOLORES EOS QUI RATIONE VOLUPTATEM SEQUI NESCIUNT.”"
    },
    {
      "role": "pullquote",
      "text": "— ATTRIBUTION"
    },
    ...
  ],
  ...
}
```

### Define Styles for Pull Quote Text

In Creating Your First Article, you applied text styles using `ComponentTextStyle` objects. Here, you’ll do something similar—create two more `ComponentTextStyle` objects so that you can apply styles to `pullquote` components.

To set the pull quote apart visually, you’ll use `hangingPunctuation`. This causes punctuation (such as opening and closing quotation marks) to appear outside of the component’s designated span.

You can also add tracking, or the horizontal spacing between letters, to take advantage of the fact that the attribution is unlikely to use the full component width.

1.  Copy the example code Pull Quote Text Styles: Copy This Code.

2.  Paste the code between the closing brace (`}`) of the last component text style and the closing brace for the whole `componentTextStyles` property.

Your code should look like the example code Pull Quote Text Styles: Result.

#### Pull Quote Text Styles: Copy This Code

```
,
    "default-pullquote": {
      "fontName": "DINAlternate-Bold",
      "fontSize": 30,
      "lineHeight": 36,
      "textColor": "#A6AAA9",
      "hangingPunctuation": true
    },
    "attribution": {
      "fontName": "DINAlternate-Bold",
      "fontSize": 12,
      "lineHeight": 16,
      "tracking": 0.12,
      "textColor": "#53585F",
      "textAlignment": "right"
    }
```

#### Pull Quote Text Styles: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "componentTextStyles": {
    ...
    "default-pullquote": {
      "fontName": "DINAlternate-Bold",
      "fontSize": 30,
      "lineHeight": 36,
      "textColor": "#A6AAA9",
      "hangingPunctuation": true
    },
    "attribution": {
      "fontName": "DINAlternate-Bold",
      "fontSize": 12,
      "lineHeight": 16,
      "tracking": 0.12,
      "textColor": "#53585F",
      "textAlignment": "right"
    }
  }
  ...
}
```

### Define Minor Adjustments for Pull Quote Positions

In Positioning Text Components, you adjusted the positions of some components using `ComponentLayout` objects. Now you’ll create two other `ComponentLayout` objects to adjust the positions of your pull quote components.

1.  Copy the example code Pull Quote Layout: Copy This Code.

2.  Paste the code between the closing brace (`}`) of the last `ComponentLayout` object and the closing brace for the whole `componentLayouts` property.

Your code should look like the example code Pull Quote Layout: Result.

#### Pull Quote Layout: Copy This Code

```
,
    "fullMarginAboveLayout": {
      "columnStart": 0,
      "columnSpan": 14,
      "margin": {
        "top": 24
      }
    },
    "halfMarginAboveQuarterBelowLayout": {
      "columnStart": 0,
      "columnSpan": 14,
      "margin": {
        "top": 12,
        "bottom": 6
      }
    }
```

#### Pull Quote Layout: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "componentLayouts": {
    ...
    "fullMarginAboveLayout": {
      "columnStart": 0,
      "columnSpan": 7,
      "margin": {
        "top": 24
      }
    },
    "halfMarginAboveQuarterBelowLayout": {
      "columnStart": 0,
      "columnSpan": 7,
      "margin": {
        "top": 12,
        "bottom": 6
      }
    }
  },
...
}
```

### Use Style and Layout Objects and Add Dividers

Now that you have defined `ComponentLayout` objects, you can use them in the `pullquote` components.

1.  Copy the example code Divider Above Pull Quote: Copy This Code.

2.  Paste the code before the opening brace (`{`) that begins the first `pullquote` component.

3.  Copy the example code Divider Below Pull Quote: Copy This Code.

4.  Paste the code after the closing brace and comma (`},`) that end the second `pullquote` component.

5.  Copy the line `"layout": "halfMarginAboveQuarterBelowLayout",`

6.  Paste the line after the first instance of `"role": "pullquote",`

7.  Copy the line `"layout": "halfMarginBelowLayout",`

8.  Paste the line after the second instance of `"role": "pullquote",`

9.  Copy the line `"textStyle": "attribution",`

10. Paste the line that you copied after the line `"layout": "halfMarginBelowLayout",`

Your code should look like the example code Pull Quote Styles and Layout: Result.

After you make these changes in your code, you can preview your working `article.json` file in News Preview to see the changes to styles and layout. For example, the vertical positioning of the pull quote components has changed, and the attribution uses a different color. You can also see the new dividers.

#### Divider Above Pull Quote: Copy This Code

```
    {
      "role": "divider",
      "layout": "fullMarginAboveLayout",
      "stroke": {
        "width": 1,
        "color": "#D5B327"
      }
    },
```

#### Divider Below Pull Quote: Copy This Code

```
    {
      "role": "divider",
      "layout": "fullMarginBelowLayout",
      "stroke": {
        "width": 1,
        "color": "#D5B327"
      }
    },
```

#### Pull Quote Styles and Layout: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    ...
    {
      "role": "divider",
      "layout": "fullMarginAboveLayout",
      "stroke": {
        "width": 1,
        "color": "#D5B327"
      }
    },
    {
      "role": "pullquote",
      "layout": "halfMarginAboveQuarterBelowLayout",
      "text": "“QUIA CONSEQUUNTUR MAGNI DOLORES EOS QUI RATIONE VOLUPTATEM SEQUI NESCIUNT.”"
    },
    {
      "role": "pullquote",
      "layout": "halfMarginBelowLayout",
      "textStyle": "attribution",
      "text": "— ATTRIBUTION"
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

### Previous

Adding an Image and Captions

### Next

Adding a Gallery of Images

## See Also

### Related Documentation

object PullQuote

The component for including a pull quote.

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

Adding an Image and Captions

Create a photo that extends to both edges of the display, with captions that appear in the article layout and in full-screen view.

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

