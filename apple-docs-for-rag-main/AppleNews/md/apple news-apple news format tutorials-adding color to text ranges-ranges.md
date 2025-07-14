

- Apple News
- Apple News Format Tutorials
-  Adding Color to Text Ranges 

Article

# Adding Color to Text Ranges

Create text in color by using HTML to refer to TextStyle objects.

## Overview

**On this page, you’ll learn how to apply text styles to ranges of characters by using HTML to refer to TextStyle objects.**

You can then edit the `TextStyle` object in one place and affect multiple ranges of text.

### Create TextStyle Objects with Different Colors

Create the `TextStyle` objects that you will refer to inline in the HTML.

1.  Copy the example code Styles with Text Color: Copy This Code.

2.  Paste the code inside your article’s `ArticleDocument.textStyles` object, inside the braces (`{}`).

Your code should look like the example code Styles with Text Color: Result.

#### Styles with Text Color: Copy This Code

```
    "lightGrayText": {
      "textColor": "#A6AAA9"
    },
    "whiteText": {
      "textColor": "#FFF"
    },
    "DINText": {
      "fontName": "DINAlternate-Bold",
      "tracking": 0.01
    },
    "mediumGrayText": {
      "textColor": "#53585F"
    }
```

#### Styles with Text Color: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "textStyles": {
    "lightGrayText": {
      "textColor": "#A6AAA9"
    },
    "whiteText": {
      "textColor": "#FFF"
    },
    "DINText": {
      "fontName": "DINAlternate-Bold",
      "tracking": 0.01
    },
    "mediumGrayText": {
      "textColor": "#53585F"
    }
  },
  ...
}
```

### Use Text Styles to Change Text Color

Create references to the TextStyle objects you just created.

1.  In your `article.json` file, ensure that each of these components has a property named `format` with a value of `"html"`: `title`, `byline`, all four `caption` components, all `body` components, and the first of the two `pullquote` components. See the example code Text Color: Result.

2.  Copy the example code Title Text: Copy This Code, and then, inside your `title` component, select the value of the `text` property and paste the copied code, replacing the existing `text` property.

3.  Copy the example code Byline Text: Copy This Code, and then, inside your `byline` component, select the value of the `text` property and paste the copied code, replacing the existing `text` property.

4.  Copy the example code Floating Caption Text: Copy This Code, and then, inside your first `caption` component, select the value of the `text` property and paste the copied code, replacing the existing `text` property.

5.  Copy the example code Body Text: Copy This Code, and then, inside your `body` component that uses the `bodyFirstDropCap` component text style, select the value of the `text` property and paste the copied code, replacing the existing `text` property.

6.  Copy the example code Pull Quote Text: Copy This Code, and then, inside your `pullquote` component, select the value of the `text` property and paste the copied code, replacing the existing `text` property.

7.  Copy the example code Gallery Caption Text: Copy This Code, and then, inside the `caption` component that follows your gallery, select the value of the `text` property and paste the copied code, replacing the existing `text` property.

8.  Copy the example code Mosaic Caption Text: Copy This Code, and then, inside the `caption` component that follows your mosaic, select the value of the `text` property and paste the copied code, replacing the existing `text` property.

9.  Copy the example code Inset Photo Caption Text: Copy This Code, and then, inside the `caption` component that accompanies your inset photo, select the value of the `text` property and paste the copied code, replacing the existing `text` property.

Your code should look like the example code Text Color: Result.

After you make these changes in your code, you can preview your working `article.json` file in News Preview to see the text ranges in color.

#### Title Text: Copy This Code

```
```

#### Byline Text: Copy This Code

```
```

#### Floating Caption Text: Copy This Code

```
```

#### Body Text: Copy This Code

```
```

#### Pull Quote Text: Copy This Code

```
```

#### Gallery Caption Text: Copy This Code

```
```

#### Mosaic Caption Text: Copy This Code

```
```

#### Inset Photo Caption Text: Copy This Code

```
```

#### Text Color: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
   ...
  "components": [
    {
      "role": "section",
      ...
      "components": [
        {
          "role": "header",
          ...
          "components": [
            {
              "role": "container",
              ...
              "components": [
                ...
                {
                  "role": "title",
                  "textStyle": "heading1Light",
                  "format": "html",
                  "layout": "halfMarginBelowLayout",
                  "text": "ARTICLE TITLE WITH INLINE TEXT STYLE REFERENCES"
                }
              ]
            }
          ]
        }
      ]
    },
    {
      "role": "section",
      ...
      "components": [
        ...
        {
          "role": "byline",
          "format": "html",
          "layout": "fullMarginBelowLayout",
          "text": "By Urna Semper"
        },
        ...
        {
          "role": "container",
          ...
          "components": [
            {
              "role": "caption",
              "format": "html",
              "layout": "fullBleedLayout",
              "text": "ABOVE: Sed ut pers piciatis unde omnis iste error sit volup tatem accusa ntium dolor emque, totam rem. (Attribution)"
            }
          ]
        },
        {
          "identifier": "body1",
          "role": "body",
          "format": "html",
          "layout": "noMarginLayout",
          "textStyle": "bodyFirstDropCap",
          "text": "Bold lead-in, cum soluta nobis est eligendi optio cumque nihil impedit quo minus id quod maxime placeat facere possimus, omnis voluptas assumenda est, dolor repellendus. Link text quibusdam et aut.Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, adipisci velit."
        },
        ...
        {
          "role": "container",
          ...
          "components": [
            {
              "role": "pullquote",
              "format": "html",
              "layout": "halfMarginAboveQuarterBelowContainedLayout",
              "text": "“QUIA CONSEQUUNTUR MAGNI DOLORES EOS QUI RATIONE VOLUPTATEM SEQUI NESCIUNT.”"
            },
            ...
          ]
        },
        ...
        {
          "role": "caption",
          "format": "html",
          "layout": "halfMarginBothLayout",
          "text": "ABOVE: A caption for the entire gallery. Individual photos in the gallery also have their own captions. (Shared attribution)"
        },
        ...
        {
          "role": "caption",
          "format": "html",
          "layout": "halfMarginBothLayout",
          "text": "ABOVE: A caption for the entire mosaic. Individual photos in the mosaic also have their own captions. (Shared attribution)"
        },
        ...
            {
              "role": "caption",
              "format": "html",
              "layout": "halfMarginBothContainedLayout",
              "text": "ABOVE: A caption for the sidebar photo. (Attribution)"
            }
          ]
        },
        ...
      ]
    }
  ],
  ...
}
```

### Previous

Creating an Inset Photo

### Next

Adding Animations

## See Also

### Related Documentation

Defining and Applying Text Styles

Define and apply custom, default, and inline text styles, or use HTML tags or Markdown syntax to style your text.

Using HTML with Apple News Format

Use HTML formatting for text components.

object TextStyle

The object for defining the text style, such as font family, size, and color, that you can apply to ranges of text.

### Advanced Design Tutorial 2: Layout and Positioning

Creating a Complex, Layered Header

Layer a title and heading in front of an image, with their colors optimized for legibility.

Creating a Floating Caption

Position a caption in the wide right margin of your article.

Creating an Inset Pull Quote

Wrap article body text around an inset pull quote.

Creating an Inset Photo

Wrap article body text around an inset photo.

Adding Animations

Use animations to affect how parts of your article come into view the first time they appear.

Adding a Scene

Control how the article’s opening section comes into view.

Viewing the Finished Article for Advanced Design Tutorial 2

See the full JSON code from this tutorial.

