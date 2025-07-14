

Web Service

# Apple News Format

Get Apple News Format reference information, and create signature content for Apple News.

## Overview

Apple News Format is the JavaScript Object Notation (JSON) format you use to create articles for Apple News.

An article created in Apple News Format can include text, images, audio, video, embedded social media, photo galleries, data tables, and interactive maps. You can enhance your article with animations, behaviors, and customized styles that let you create a unique look for your content. Your finished article is processed and rendered in Apple News.

With Apple News Format, you only have to author your content once. News automatically optimizes your articles for iPhone, iPad, Mac, and Apple Vision Pro to give your readers the best experience for their device.

## Topics

### Release Notes

Release notes announce new features, updates, and deprecations for major and beta releases, so you can plan for changes and make adjustments as needed.

Apple News Format Release Notes for iOS 17, iPadOS 17, and macOS 14

Learn about new features that require iOS 17, iPadOS 17, and macOS 14.

Apple News Format Version History

Learn how Apple News Format versions map to iOS, iPadOS, macOS, and visionOS releases.

### Essentials

JSON Concepts and Article Structure

Understand basic JSON concepts and become familiar with the structure of an Apple News Format article.

Creating an Article: Main Steps

Plan the design for your article and create it in Apple News Format.

object ArticleDocument

The root object of an Apple News article, that contains required properties, metadata, content, layout, and styles.

### Article Display

Changing the Appearance of Your Article Tile in Feeds

Change the information that News displays about your published article.

### Article Metadata

object Metadata

Information about your article, including author name, creation date, publication date, keywords, and excerpt.

object LinkedArticle

A relationship between your article and another Apple News article.

object Issue

The object for defining information about an issue.

### Article Layout

Planning the Layout for Your Article

Define a layout that supports the look you want for your article.

Positioning the Content in Your Article

Align article components with columns in your layout.

Wrapping Text Around a Component

Define the layout of a text component to wrap around another component.

object Layout

The object for defining columns, gutters, and margins for your article’s designed width.

object ComponentLayout

The object for defining the positioning for a specific component within the article’s column system.

object Anchor

The object for anchoring one component to another component in your article’s layout.

object Margin

The object for defining the space above and below a component.

object AutoPlacementLayout

The object for defining the margin above and below advertising components.

object AdvertisingLayout

The object for defining the margin above and below advertising components.

Deprecated

### Article Content

Components

Understand the types of components that can make up an article.

### Styles

Enhancing Your Articles with Styles

Improve the appearance of the text and components in your article by using Apple News Format styles.

Supporting Dark Mode for Your Article

Update your article template so that your article adapts when Dark Mode is active.

object DocumentStyle

The object for setting the background color for your article.

Text Styles

Learn about text styles and how to apply them to your text and text components.

Component Styles

Learn to use component styles to add borders, set background colors, and apply background images to components and to set the styling for tables.

Supported Color Names

Learn the color names supported in Apple News Format.

type Color

The strings for defining colors in Apple News Format.

### Dynamic Advertising

Managing Advertisements in Your Channel

Set the layout and frequency of ads automatically inserted in an article.

object AutoPlacement

The object for automatically placing components within Apple News Format articles.

object AdvertisementAutoPlacement

The object for defining the automatic placement of advertisements.

object AdvertisingSettings

The object for defining properties that affect the frequency and placement with which banner advertisements and medium rectangle advertisements are automatically placed in your article.

Deprecated

### Conditional Design Elements

Define conditions for various objects to get the right look for your content.

object Condition

The object for defining a condition that, when met, causes conditional properties to go into effect.

object ConditionalComponent

The object for defining conditional properties for a component, and when the conditional properties are in effect.

object ConditionalComponentLayout

The object for defining conditional properties for a component layout, and when the conditional properties are in effect.

object ConditionalAutoPlacement

The object for defining conditional properties for an automatically placed component, and when the conditional properties are in effect.

object ConditionalSection

The object for defining conditional properties for a section component, and when the conditional properties are in effect.

object ConditionalDocumentStyle

The object for defining conditional properties for a document style, and when the conditional properties are in effect.

object ConditionalText

The object for defining conditional properties for a text component, and when the conditional properties are in effect.

object ConditionalTextStyle

The object for defining conditional properties for a text style, and when the conditional properties are in effect.

object ConditionalComponentTextStyle

The object for defining conditional properties for a component text style, and when the conditional properties are in effect.

object ConditionalComponentStyle

The object for defining conditional properties for a component style, and when the conditional properties are in effect.

object ConditionalContainer

The object for defining conditional properties for a container component, and when the conditional properties are in effect.

object ConditionalDivider

The object for defining conditional properties for a divider component, and when the conditional properties are in effect.

object ConditionalButton

The object for defining a button component’s conditional properties, and when the conditional properties are in effect.

### Component Measurements and Media Guidelines

Specifying Measurements for Components

Specify the units of measure to use for margins, minimum heights, and other dimensions.

type SupportedUnits

The units of measurement Apple News Format supports.

Preparing Image, Video, Audio, Music, and ARKit Assets

Add media assets to your article.

