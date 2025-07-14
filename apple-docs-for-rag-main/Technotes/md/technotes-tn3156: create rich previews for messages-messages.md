

- Technotes
-  TN3156: Create rich previews for Messages 

Article

# TN3156: Create rich previews for Messages

Learn best practices for creating rich text and image previews for display in the Messages app.

## Overview

The Messages app on iOS and macOS by default shows inline previews for links as gray bubbles with the page title, domain, and small icon belonging to the linked web page:

You can display images and meaningful captions in these link previews by adding Open Graph metadata on your website pages. Here’s an example link preview for `https://www.apple.com/iphone`, which includes an image and title:

This appearance results from the following `meta` tags on the webpage:

```
```

Read the following sections for tips on how to get rich link previews in Messages.

## Use consistent metadata for all user agents

Serve the same metadata to both mobile and desktop versions of the page. Clients shouldn’t have to change the `User-Agent` header to receive useful metadata.

## Add images to link previews

Use the `og:image` property to include an image in your link preview. Preview images are displayed large enough to represent the linked page clearly, including relevant details.

Also provide a high-resolution icon in addition to your image. The link preview will use an apple-touch-icon, a favicon, or an icon specified by ``. If you do not have a preview image of sufficient size or quality, use an `apple-touch-icon` instead.

Avoid text in preview images. Images may be displayed at varying sizes depending on context and device, potentially making text unreadable. For best results, keep the image graphical and use other metadata tags for text. Text provided via metadata is also accessible for people using VoiceOver.

## Add videos to link previews

If you want to display a video in your preview, use a direct link to your video asset via a `meta` tag, rather than a reference to an embeddable video page. With the direct link, the video loads and displays faster, and it uses the system user interface for playback.

If the link preview encounters an `og:video` or `twitter:player:stream` property that points to a downloadable and playable media asset (for example, an MPEG-4 file), the preview downloads the video and automatically plays it back.

Videos that can be streamed but not downloaded, such as HTTP Live Streaming (HLS) streams, require the user to tap to start playback. Videos that require embedding HTML will not play inline.

## Customize titles in link previews

Use the `og:title` property to specify the title of your link preview. Titles should be short and specific enough to distinguish different pages on the same website. For example, product pages should indicate the product name in the title.

Do not put the site name or other branding in the `og:title`. Doing so often leads to duplication of information between the title and other parts of the rich preview, and is semantically incorrect. Use `og:site_name` for the site name instead.

## Ensure your metadata is reachable

Link previews do not follow `meta` redirects, nor run JavaScript; metadata must be available directly on the linked page. Server-side redirects are followed, however, and are a good alternative.

Pages that require authentication should still have meaningful metadata, without revealing any sensitive content. For pages that require authentication, the main resource should provide metadata for the page to which access is being provided, and not for the authentication page itself. This avoids showing “Sign In” as the title for every page behind an authentication wall.

## Respect resource usage guidelines

- Icons should be square, at least 108 pixels per side.

- Images should be at least 900 pixels in width.

- Images less than 150 pixels in width may be ignored or presented as icons.

- The main resource located at the previewed link is limited to 1 MB. The total size of associated resources (icons, images, and videos, etc) is limited to 10 MB.

These recommendations are guidelines only. Limits may change in the future.

## Enable social network link previews

For preview links to user posts on social network services, specify the text of the user post via the `og:description` property. In addition:

- The page must be configured with a `twitter:card` value of `summary` or `summary_large_image` as described in the X for Websites documentation.

- The page must have a `link` element with a `type` attribute of `application/activity+json` as described in the ActivityPub protocol documentation.

## Revision History

- **2024-04-30** Republished as TN3156. Added social network information.

- **2017-09-08** First published as TN2444 “Best Practices for Link Previews in Messages”.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

