

- Apple News
- Apple News Format Tutorials
-  Adding a Podcast 

Article

# Adding a Podcast

Add a link to a podcast that displays the podcast artwork and the podcast show or episode information.

## Overview

By using the podcast component, you can add a link to a podcast without using external assets.

**On this page, you’ll learn how to**:

- Create a podcast component.

- Change the podcast orientation.

### Add a Podcast in Your Article

In Positioning Text Components, you created some `ComponentLayout` objects. You’ll refer to those `ComponentLayout` objects in this code.

1.  Copy the example code from Podcast: Copy This Code.

2.  Paste the code inside the components array of your article, after the closing brace and comma (`},`) of the body component that begins with `Consequatur` `aut doloribus`.

Your code should look like the example code in Podcast: Result.

After you make this change in your code, you can preview your working `article.json` file in News Preview to see a podcast in your article.

#### Podcast: Copy This Code

```
    {
      "role": "heading2",
      "layout": "fullMarginAboveHalfBelowLayout",
      "text": "PODCAST HEADING"
    },
    {
      "role": "podcast",
      "layout": "noMarginLayout",
      "URL": "https://podcasts.apple.com/us/podcast/apple-news-today/id1473872585"
    },
```

#### Podcast: Result

Ellipses (…) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    ...
    {
      "role": "heading2",
      "layout": "fullMarginAboveHalfBelowLayout",
      "text": "PODCAST HEADING"
    },
    {
      "role": "podcast",
      "layout": "noMarginLayout",
      "URL": "https://podcasts.apple.com/us/podcast/apple-news-today/id1473872585"
    },
    ...
  ],
  ...
}
```

### Adjust the Podcast Orientation

The podcast you added to your article shows the default podcast orientation that changes automatically based on screen size. On larger tablet screens, the podcast art displays on the left and the podcast information and link button appear on the right. On smaller mobile screens, the artwork, podcast information, and link button appear stacked.

Instead of using the orientation that automatically changes based on screen size, you can set the default orientation to `lanndscape`. The `landscape` orientation saves screen space on mobile devices.

1.  Copy the line `"orientation": "landscape"`,

2.  Paste the line inside your `podcast` component, after the line that begins with `"layout"`:

After you make this change in your code, you can preview your working `article.json` file in News Preview to see a podcast set to `landscape` orientation.

#### Podcast Orientation: Result

Ellipses (…) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    ...
    {
      "role": "heading2",
      "layout": "fullMarginAboveHalfBelowLayout",
      "text": "PODCAST HEADING"
    },
    {
      "role": "podcast",
      "layout": "noMarginLayout",
      "orientation": "landscape",
      "URL": "https://podcasts.apple.com/us/podcast/apple-news-today/id1473872585"
    },
    ...
  ],
  ...
}
```

#### Previous

Adding a Tweet

#### Next

Viewing the Finished Article for the Introductory Design Tutorial

## See Also

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

Adding a Tweet

Include a tweet in an article.

Viewing the Finished Article for the Introductory Design Tutorial

See the full JSON code from this tutorial.

