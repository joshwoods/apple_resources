

- Apple News
- Apple News Format Tutorials
-  Adding a Tweet 

Article

# Adding a Tweet

Include a tweet in an article.

## Overview

A `tweet` component lets users see social media content in an article.

**On this page, you’ll learn how to use a tweet component to embed a tweet in an article.**

### Add a Tweet in Your Article

In Positioning Text Components, you created some `ComponentLayout` objects. You’ll refer to those `ComponentLayout` objects in this code.

1.  Copy the example code Tweet: Copy This Code.

2.  Paste the code inside in the `components` array of your article, after the last component and before the closing square bracket (`]`) at the end of the array.

Your code should look like the example code Tweet: Result.

After you make this change in your code, you can preview your working `article.json` file in News Preview to see a tweet in your article.

#### Tweet: Copy This Code

```
,
    {
      "role": "heading2",
      "layout": "fullMarginAboveHalfBelowLayout",
      "text": "TWEET HEADING"
    },
    {
      "role": "tweet",
      "layout": "noMarginLayout",
      "URL": "https://twitter.com/Urna_Semper/status/1480968065630285834"
    }
```

#### Tweet: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    ...
    {
      "role": "heading2",
      "layout": "fullMarginAboveHalfBelowLayout",
      "text": "TWEET HEADING"
    },
    {
      "role": "tweet",
      "layout": "noMarginLayout",
      "URL": "https://twitter.com/Urna_Semper/status/1480968065630285834"
    }
  ],
  ...
}
```

### Further Exploration

At any time, you can try changing property values in your `article.json` file and then use News Preview to see how these changes affect the look of your article.

For example, try changing which tweet appears in your article:

1.  In your `article.json` file, find the `tweet` component.

2.  Replace the value of the component’s `URL` property (`"https://twitter.com/Urna_Semper/status/1480968065630285834"`) with the URL to another tweet.

3.  Preview your `article.json` file in News Preview.

The article now shows the tweet that you chose.

### Previous

Adding a Mosaic of Images

### Next

Adding a Podcast

## See Also

### Related Documentation

object Tweet

The component for adding a Tweet that was posted to Twitter.

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

Adding a Pull Quote

Break an existing body component into two components, and then insert a pull quote between them.

Adding a Gallery of Images

Display three images as a sequential gallery.

Adding a Mosaic of Images

Display five images as mosaic tiles.

Adding a Podcast

Add a link to a podcast that displays the podcast artwork and the podcast show or episode information.

Viewing the Finished Article for the Introductory Design Tutorial

See the full JSON code from this tutorial.

