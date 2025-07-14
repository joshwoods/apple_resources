

- Apple News
- Apple News Format
-  Changing the Appearance of Your Article Tile in Feeds 

Article

# Changing the Appearance of Your Article Tile in Feeds

Change the information that News displays about your published article.

## Overview

Every article you publish has an article tile that provides information about the article. The article tile appears in the topic and channel feeds and in the reader’s For You feed.

Your article tile can incorporate information from your ArticleDocument properties, your article Metadata, your Create an Article request, and your channel name.

To change the different parts of your article tile, modify the following properties:

- `thumbnailURL`, `videoURL`. Use the `thumbnailURL` property in the article’s Metadata object to specify the image you want to use in the article tile. Optionally specify the `videoURL` property. When you provide both `thumbnailURL` and `videoURL`, Apple News displays the `videoURL` in the article tile. See Preparing Image, Video, Audio, Music, and ARKit Assets.

- `title`. Use the `title` property in the ArticleDocument object to specify the article’s title.

- `datePublished,dateModified`. Use the `datePublished` or `dateModified` property in the article’s Metadata object to specify the date the article was published or most recently modified (after publication).

- `authors`. Use the `authors` property in the article’s Metadata object to specify the author of the article. This text appears below the headline in your article tile.

- `excerpt`. Use the `excerpt` property in the article’s Metadata object to specify the summary or the subheadline. Although it’s optional, try to include an excerpt for all of your articles and keep within the recommended 80–300 character range. This text may appear in the article tile in feeds or when an article is shared. Don’t use HTML tags or Markdown syntax for this property.

