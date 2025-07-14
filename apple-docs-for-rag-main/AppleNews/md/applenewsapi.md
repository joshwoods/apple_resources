

Web Service

# Apple News API

Publish and manage Apple News Format articles.

## Overview

The Apple News API delivers Apple News Format articles to be published in the Apple News app and helps you manage and monitor those articles after they’ve been published.

Based on representational state transfer (REST) technology, the Apple News API has typical RESTful characteristics, which means that it:

- Does operations on a set of resources. Resources are objects that have a type, associated data, and relationships to other resources. In the Apple News API, resources include channels, sections that you’ve set up for your channels (for example, Sports or Politics), and the articles that you want to publish and manage.

- Has stateless operations. Interactions with the create, read, update, and delete (CRUD) operations are handled using only the information that comes with the request — no previous information or state is assumed. Therefore, requests made using the Apple News API must include all information required to complete the operation within the request.

## Topics

### Essentials

Getting Ready to Publish and Manage Your Articles

Get set up for using the Apple News API.

About the Apple News Security Model

Learn how the Apple News API authenticates clients, authorizes your news channel, and enforces confidentiality.

About Apple News API Field Types

Understand the standard field types used in the Apple News API.

Formatting Strings

Learn how to format strings to pass to the API client.

### Release Notes

Release notes announce new features, updates, and deprecations for major releases, so you can plan for changes and make adjustments as needed.

Apple News API Release Notes for iOS 17, iPadOS 17, and macOS 14

Learn about the new features and deprecated fields in Apple News API.

### Channel

Read Channel Information

Get details about your channel, including the name, corresponding website, and default section.

Read Channel Quota Information

Get details about your channel’s remaining quota for sending create and update requests, the queue size, and wait time.

object Channel

See the fields the read channel endpoint returned.

object ChannelLinks

See the links the read channel endpoint returned.

object ChannelResponse

See which objects make up the channel response.

### Sections

List All Sections

See a list of available sections in your channel.

Read Section Information

Get information about the specified section, including its name, its channel, and whether it’s a default section.

Promote Articles in a Section

Set the list of promoted articles for the specified section.

object Section

See the fields the section endpoints returned.

object SectionLinks

See the links the section endpoints returned.

object SectionResponse

See which objects make up the section response.

object PromoteArticleRequest

See the required field for the Promote an Article request.

object PromoteArticleResponse

See the field the Promote an Article response returned.

### Articles

Create an Article

Publish an article to your channel.

Read Article Information

Retrieve information about an article, such as the revision number and maturity rating.

Search Articles in a Channel

See a list of all articles in a channel that match the specified search criteria.

Search Articles in a Section

See a list of all articles in a section that match the specified search criteria.

Update an Article

Update an existing article in your channel.

Delete an Article

Delete the specified article from your channel.

object Create Article Metadata Fields

See the optional metadata fields for the Create an Article Request.

object ArticleLinksRequest

See the required field for the Create an Article request.

object Update Article Metadata Fields

See the metadata fields for the Update an Article request.

object Article

See the fields the article endpoints returned.

object ArticleResponse

See which objects make up the Create an Article, Read an Article, and Update an Article responses.

object ArticleLinksResponse

See the links the article endpoints returned.

object SearchResponse

See the fields the search article endpoints returned.

object Meta

See the object that wraps the throttling information that’s returned for the Create an Article and Read an Article endpoints.

object Throttling

See the object that wraps the throttling information that’s returned for the Create an Article and Update an Article endpoints.

### Errors

About Apple News API Error Messages

Understand the error message format for the Apple News API.

object Warning

See the properties of a warning the Apple News API returned.

object Error

See the properties of an error the Apple News API returned.

type Code

See the error codes the Apple News API returned.

type Status

See the HTTP status codes the Apple News API returned.

