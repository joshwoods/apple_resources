

- Apple News
- Apple News Format
-  Components 

API Collection

# Components

Understand the types of components that can make up an article.

## Overview

Components are some of the main objects you use to build your article, along with layouts and styles. Components hold the content of your article and are always in an array called `components`.

Each component in your article has a function that is expressed by a property called `role`. For example, the value of the `role` property might be `title`, `body`, `pullquote`, or `heading`. A component’s role determines what type of component it is. That is, when a component’s `role` is `body`, that type of component is referred to as a `body` component. See JSON Concepts and Article Structure.

The following table gives you an overview of the components you can use to create an article in Apple News Format.

| **Component category** | **Component types** |
|----|----|
| Text | Body, Title, Heading (heading1, heading2, heading3, heading4, heading5, heading6), ArticleTitle, Intro, Caption, Author, Byline, Illustrator, Photographer, Quote, PullQuote |
| Images | Image, Photo, Figure, Portrait, Logo, ArticleThumbnail |
| Galleries and Mosaic | Gallery, Mosaic |
| Audio and Video | Audio, EmbedWebVideo, Music, Podcast, Video |
| Location | Map, Place |
| Social Media | FacebookPost, Instagram, TikTok, Tweet |
| Tables | DataTable, HTMLTable |
| Advertisements | ReplicaAdvertisement |
| Article Structure | Container, Section, Chapter, Aside, Header, Divider, ArticleLink, LinkButton |
| Augmented Reality | ARKit |

Note

Choosing the component `role` that best describes your content is important for better voice-over and for facilitating Siri suggestions. For example, instead of styling text in a `body` component to make it look like a heading, use a `heading` component for that text instead.

## Topics

### First Steps

Adding Components

Learn the basics for adding components to your article.

object Component

Properties shared by all component types.

### Text

Using HTML with Apple News Format

Use HTML formatting for text components.

Using Markdown with Apple News Format

Use Markdown formatting for text components.

object Body

The component for adding body text.

object Title

The component for adding an article title.

object Heading

The text component for adding a heading.

object Intro

The component for adding introductory text.

object Caption

The component for adding caption text.

object Author

The component for adding the name of the author.

object Byline

The component for adding the publication date or contributor credits, especially for articles with multiple contributors.

object Illustrator

The component for adding illustrator credit.

object Photographer

The component for adding a photographer credit.

object Quote

The component for including a quote.

object PullQuote

The component for including a pull quote.

object Text

Properties shared by all text component types.

### Images

object Image

The component for displaying JPEG, WebP, PNG, or GIF images.

object Photo

The component for including a photograph.

object Figure

The component for including a figure.

object Portrait

The component for including an image of a person.

object Logo

The component for including a logo image.

object ReplicaAdvertisement

The component for delivering digital versions of print advertisements.

object CaptionDescriptor

The object you use in image components for displaying captions when the image is full-screen.

### Galleries and Mosaics

object Gallery

The component for displaying a sequence of images in a specific order as a horizontal strip.

object Mosaic

The component for displaying a set of images as tiles in no particular order.

object GalleryItem

An object used in a gallery or mosaic component for displaying an individual image.

### Audio and Video

object Audio

The component for adding a playable audio clip.

object Music

The component for adding a playable music file.

object Podcast

The component for adding a Podcast show or episode.

object Video

The component for adding a video.

object EmbedWebVideo

The component for adding a web video from Dailymotion, Vimeo, or YouTube.

### Location

object Map

The component for adding a map.

object MapItem

An object used in a map component for specifying the location of a map pin.

object MapSpan

An object used in a map or place component for defining the visible area of the map.

object Place

The component for adding a map with a specific point of interest.

### Social Media

object Instagram

The component for adding an Instagram post.

object FacebookPost

The component for adding a Facebook post.

object TikTok

The component for adding a TikTok post.

object Tweet

The component for adding a Tweet that was posted to Twitter.

### Augmented Reality

object ARKit

The component for adding an augmented reality (AR) experience to your article.

### Tables

Tables in an Article

Add a JSON or HTML data table, and understand the options for changing the look of your table.

### Advertisements

object BannerAdvertisement

The component for adding a full-width banner ad.

Deprecated

object MediumRectangleAdvertisement

The component for adding a medium, fixed-size rectangle ad.

Deprecated

### Article Structure

Nesting Components in an Article

Use container components to create the component hierarchies you need for special article designs.

Adding a Scene to a Chapter or a Section Header

Add a scene to your article to create special effects.

Creating an Article Link

Link to an article by using the article-linking container component.

Displaying Components Side By Side

Configure a side-by-side, horizontal arrangement of components for your article.

object Header

The component for defining the top area of an article, chapter, or section.

object Container

Properties shared by all container types.

object Section

The component for organizing an article into sections.

object Chapter

The component for organizing an article into chapters.

object Aside

The component for setting apart content that is not directly related to the article, such as promotional content.

object CollectionDisplay

An object used in any container component type to define how the collection of child components is presented.

object HorizontalStackDisplay

The object for displaying components side by side in a Container component.

object FlexibleSpacer

The component for redistributing empty space inside a horizontal stack collection.

object Divider

The component for defining a horizontal line to visually divide parts of your article.

object ArticleLink

The container component for creating a link to an article.

type SupportedArticleIdentifier

The patterns supported for article identifiers in UUID format.

type PublisherArticleIdentifier

The identifier provided by the publisher.

object ArticleTitle

The component for displaying an article title in the ArticleLink component.

object ArticleThumbnail

The component for displaying a thumbnail image with an article link.

object LinkButton

The component for opening a link in a button.

### Animations

About Component Animations

Learn how to affect the way in which components come into view.

object ComponentAnimation

Properties that all types of animations share.

object AppearAnimation

An animation type whereby a component appears on the screen.

object FadeInAnimation

The animation whereby a component fades into view.

object MoveInAnimation

The animation whereby a component moves in from the side of the screen.

object ScaleFadeAnimation

The animation in which a component scales up and fades into view.

### Behaviors

About Component Behaviors

Learn how to affect components’ reactions to device motion and scrolling.

object Behavior

Properties shared by all the behaviors you can use to affect how components react to device motion and scrolling.

object BackgroundMotion

The behavior whereby the background of a component moves in the opposite direction from the motion of the device.

object BackgroundParallax

The behavior whereby the background of a component moves slightly slower than a person’s scroll speed.

object Motion

The behavior whereby a component reacts to the motion of the person’s device.

object Parallax

The behavior whereby a component moves at a speed different from the scroll speed.

object Springy

The behavior whereby a component acts as if it’s on a short spring.

### Links

object LinkAddition

The addition object for defining links in text components that don’t use HTML or Markdown formatting.

object ComponentLink

The component addition object for making a component interactive and opening a link to another location in News.

object Addition

Properties that all addition types share.

object ComponentAddition

Properties that all types of component additions share.

type SupportedURLs

Links that go to Apple News, other Apple apps, and external sites.

type SupportedInternalURLs

Links that go to Apple News and other Apple apps.

