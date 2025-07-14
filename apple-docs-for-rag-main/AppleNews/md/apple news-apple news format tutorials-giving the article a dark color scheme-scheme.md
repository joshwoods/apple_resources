

- Apple News
- Apple News Format Tutorials
-  Giving the Article a Dark Color Scheme 

Article

# Giving the Article a Dark Color Scheme

Apply a new color scheme to your article.

## Overview

In this third advanced article design, you’ll create some visual effects using a dark color scheme, a `video` component, and a fixed image fill.

**On this page, you’ll learn how to use ComponentStyle objects to implement a color scheme**.

### Define a Dark Background Color for Components

You can use a dark color scheme to create contrast between one group of articles and another or for variety within a single article.

This `ComponentStyle` object has a dark background color.

1.  Open the `article.json` file that you completed in Adding a Scene, or open `Desktop/News_Design_Tutorial/News_Design_Tutorial_Advanced_Article_2/article.json`.

2.  Copy the example code darkBackgroundStyle: Copy This Code.

3.  Paste the code between the closing brace (`}`) of the last `ComponentStyle` object and the closing brace for the whole `componentStyles` property.

Your code should look like the example code darkBackgroundStyle: Result.

#### darkBackgroundStyle: Copy This Code

```
,
    "darkBackgroundStyle": {
      "backgroundColor": "#202020"
    }
```

#### darkBackgroundStyle: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "componentStyles": {
    ...
    "darkBackgroundStyle": {
      "backgroundColor": "#202020"
    }
  },
  ...
}
```

### Define a Light-Color Text Style

The `ComponentTextStyle` object called `bodyFirstDropCapDark` has a light text color.

1.  Copy the example code bodyFirstDropCapDark: Copy This Code.

2.  Paste the code inside the `ArticleDocument.componentTextStyles` object in your `article.json` file, after the closing brace (`}`) of the last text style and before the closing bracket for the whole `componentTextStyles` property.

Your code should look like the example code bodyFirstDropCapDark: Result.

#### bodyFirstDropCapDark: Copy This Code

```
,
    "bodyFirstDropCapDark": {
      "textColor": "#FFF",
      "dropCapStyle": {
        "fontName": "DINAlternate-Bold",
        "textColor": "#D5B327",
        "numberOfLines": 2
      }
    }
```

#### bodyFirstDropCapDark: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "componentTextStyles": {
    ...
    "bodyFirstDropCapDark": {
      "textColor": "#FFF",
      "dropCapStyle": {
        "fontName": "DINAlternate-Bold",
        "textColor": "#D5B327",
        "numberOfLines": 2
      }
    }
  }
}
```

### Implement the Dark Color Scheme

You’ll move some components from the header into a new section and add references to a new `ComponentStyle` object and a new `ComponentTextStyle` object.

1.  In your `article.json` file, delete the contents of your header’s `components` array. The code you’re deleting begins with the opening brace (`{`) before `"role": "container"`, and ends with a mix of three alternating brackets and braces (`}]}`).

2.  Copy the example code Components: Copy This Code.

3.  Paste the code inside your second section’s `components` array, after the opening bracket (`[`).

4.  Copy the example code Section Boundary: Copy This Code.

5.  Paste the code inside your second section, replacing the comma that follows the first body component.

6.  In your second section, change the value of `style` to `"darkBackgroundStyle"`.

7.  In your floating caption, add a `textStyle` property with a value of `"captionLight"`.

8.  In the body component that uses `bodyFirstDropCap`, change the value of `textStyle` to `"bodyFirstDropCapDark"`, and change the value of `layout` to `"fullMarginBelowLayout"`.

Your code should look like the example code Dark Color Scheme: Result.

After you make these changes in your code, you can preview your working `article.json` file in News Preview to see the dark color scheme.

#### Components: Copy This Code

```
        {
          "role": "heading1",
          "layout": "heading1Layout",
          "text": "HEADING"
        },
        {
          "role": "divider",
          "layout": "bigDividerLayout",
          "stroke": {
            "width": 3,
            "color": "#D5B327"
          }
        },
        {
          "role": "title",
          "format": "html",
          "layout": "halfMarginBelowLayout",
          "text": "ARTICLE TITLE WITH INLINE TEXT STYLE REFERENCES"
        },
```

#### Section Boundary: Copy This Code

```
]
    },
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "style": "bodyBackgroundStyle",
      "components": [
```

#### Dark Color Scheme: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "scene": {
        "type": "fading_sticky_header",
        "fadeColor": "#000"
      },
      "components": [
        {
          "role": "header",
          "layout": "headerImageLayout",
          "style": {
            "fill": {
              "type": "image",
              "URL": "bundle://header.jpg",
              "fillMode": "cover",
              "verticalAlignment": "top",
              "horizontalAlignment": "center"
            }
          }
        }
      ]
    },
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "style": "darkBackgroundStyle",
      "components": [
        {
          "role": "heading1",
          "layout": "heading1Layout",
          "text": "HEADING"
        },
        {
          "role": "divider",
          "layout": "bigDividerLayout",
          "stroke": {
            "width": 3,
            "color": "#D5B327"
          }
        },
        {
          "role": "title",
          "format": "html",
          "layout": "halfMarginBelowLayout",
          "text": "ARTICLE TITLE WITH INLINE TEXT STYLE REFERENCES"
        },
        ...
        {
          "identifier": "body1",
          "role": "body",
          "format": "html",
          "layout": "fullMarginBelowLayout",
          "textStyle": "bodyFirstDropCapDark",
          "text": "Bold lead-in, cum soluta nobis est eligendi optio cumque nihil impedit quo minus id quod maxime placeat facere possimus, omnis voluptas assumenda est, dolor repellendus. Link text quibusdam et aut.Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, adipisci velit."
        }
      ]
    },
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "style": "bodyBackgroundStyle",
      "components": [
        {
          "role": "heading2",
          "layout": "fullMarginAboveHalfBelowLayout",
          "text": "HEADING"
        },
        ...
      ]
    }
  ],
  ...
}
```

### Set the Default to a Dark Color Scheme

To view the dark color scheme in Dark Mode, switch your simulator device to a dark systemwide appearance (Features \> Toggle Appearance).

You can maintain the dark color scheme for your article even when a user switches between a light or dark appearance. Set the `preferredColorScheme` conditional to define the background color for a specific appearance. For more information about conditionals, see Apple News Format \> Condition.

In Define a Dark Background Color for Components, you created a new `ComponentStyle` called `darkBackgroundStyle`. Now you’ll update that style with a conditional to explicitly set a value for your article’s dark appearance.

1.  Copy the example code from Condition Dark Mode: Copy This Code.

2.  Paste the code inside the `darkBackgroundStyle`, `componentStyle` of your article, at the end of this line: `"backgroundColor": "#202020"`.Your code should look like the example code in Condition Dark Mode: Result.

#### Condition Dark Mode: Copy This Code

```
,
"conditional": [
  {
    "backgroundColor": "#202020",
    "conditions": [
      {
        "preferredColorScheme": "dark"
      }
    ]
  }
]

```

#### Condition Dark Mode: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{  ...
  "componentStyles": {
    ...
     "darkBackgroundStyle": {
      "backgroundColor": "#202020",
      "conditional": [
        {
          "backgroundColor": "#202020",
          "don’tions": [
            {
              "preferredColorScheme": "dark"
            }
          ]
        }
      ]
    },
    ...
}
```

To view the dark color scheme when the device appearance is toggled, preview your working `article.json` file in News Preview.

**Light Appearance**

**Dark Appearance**

### Further Exploration

For information about using Dark Mode and adjusting designs for light and dark appearances, see Apple Human Interface Guidelines > Dark Mode.

For information about updating your article so that it adapts when Dark Mode is active, see Supporting Dark Mode for Your Article.

### Previous

Viewing the Finished Article for Advanced Design Tutorial 2

### Next

Adding a Video

## See Also

### Related Documentation

Applying a Background to a Component

Change the appearance of the backgrounds in your article.

Defining a Component Style

Set style options for the components in your article.

object ComponentStyle

The object for setting style properties for components, including background color and fill, borders, and table styles.

object TextStyle

The object for defining the text style, such as font family, size, and color, that you can apply to ranges of text.

### Advanced Design Tutorial 3: More Ideas

Adding a Video

Add a video component inside the header component.

Creating a Sidebar

Create a box with an HTML bulleted list in the margin.

Adding a Fixed Image Fill

Add an image that remains stationary when the user scrolls.

Creating a Newsletter Sign-Up Element

Add a newsletter sign-up element in your article.

Viewing the Finished Article for Advanced Design Tutorial 3

See the full JSON code from this tutorial.

