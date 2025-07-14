

- Apple News
- Apple News Format
-  Creating an Article: Main Steps 

Article

# Creating an Article: Main Steps

Plan the design for your article and create it in Apple News Format.

## Overview

When you create an article in Apple News Format, you start by creating a JSON document file. The file contains code that specifies the layout for your article, provides the content, and customizes the look. The system processes the JSON file and renders it as an article in Apple News.

Your article in Apple News must contain the following:

- A headline for the article. Use the Title component.

- An author for the article. Use the Author component to include the name of one of the authors of the article. Alternatively, you can use the Byline component for adding contributors to your article.

- The publication date of the article. Use either the Metadata, `datePublished` property or the Byline component.

- The complete text of the article, as it appears in either print or on the publisher’s website. Use the Body component. Don’t truncate articles or require people to leave the Apple News app to read the full story.

You can also include a thumbnail URL to use in the article tile. See the Metadata, `thumbnailURL` property.

Avoid using generic banners or branding messages at the top of articles, because the system automatically brands articles with channel names. Redundant branding pushes down the article’s content, forcing people to scroll to view it.

You can include in-article modules to promote and support your publication, like channel follow buttons, newsletter sign-up calls, donations, and other campaigns, but they must not appear until after the first screen.

Modules that promote other products and services, advertising, or commercial content are prohibited.

The following figure shows the basic tasks associated with creating an article.

### Main Steps

Note

Before you start, download News Preview and follow the instructions to choose the devices you want to preview on. Then, as you create your article, you can drag your `article.json` file to the News Preview window to see how your content will look in Apple News.

1.  **Create an** `article.json` **document file**. All article document files must have the name `article.json.` Start by adding the ArticleDocument object and its required properties, or download this sample file. You can use any text editor to edit the code in your `article.json` file. See Choose a Text Editor. Create a unique folder to hold the `article.json` file and any other files you’ll publish with this article, such as image files.

2.  **Plan the layout of your article**. Decide how many layout columns your design needs. See Planning the Layout for Your Article.

3.  **Add components that contain your article’s content**. The content of your article — the text, photos, and other information — is contained in an array of components in your `article.json` file. Each component has a specific function — for example, a title, a caption, body text, or a video. For an overview of the different kinds of components you can have in your article, see Components; to learn how to add components, see Adding Components.

4.  **Position the components in your article**. Use the ComponentLayout object to specify where each component will appear horizontally in your article document. See Positioning the Content in Your Article.

5.  **Customize the appearance of your article**. Include styles, animations, behaviors, and other effects. See Enhancing Your Articles with Styles and About Component Animations.

6.  **Add the metadata for your article**. See Metadata.

Once your article is finished, you can publish it to Apple News. See Create an Article.

## See Also

### Essentials

JSON Concepts and Article Structure

Understand basic JSON concepts and become familiar with the structure of an Apple News Format article.

object ArticleDocument

The root object of an Apple News article, that contains required properties, metadata, content, layout, and styles.

