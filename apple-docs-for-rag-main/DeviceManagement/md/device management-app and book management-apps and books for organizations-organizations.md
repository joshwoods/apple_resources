

- Device Management
- App and Book Management
-  Apps and Books for Organizations 

API Collection

# Apps and Books for Organizations

Get details about apps and books to show to your users.

## Overview

Use the Apps and Books for Organizations API to retrieve metadata for apps and books that your organization owns, or to search for and retrieve metadata for apps and books in the public catalog.

This API requires authentication that you’re a member of the Apple Developer Program and a trusted developer. Each request requires a signed developer token as a header. Requests for apps and books your organization owns also require your organization’s `sToken` as a cookie.

## Topics

### Essentials

Generating developer tokens

Create a JSON Web Token to authorize your requests to the Apps and Books for Organizations API.

Handling requests and responses

Write a request for app or book metadata and handle responses from the API.

Fetching resources with extended attributes

Specify additional attributes for the API to include in a response.

Fetching storefront objects

Pick a region-specific geographic location to retrieve catalog information from.

Common Objects

Understand the common JSON objects that framework responses contain.

### App and book metadata

Get Metadata for Your Apps

Fetch metadata for your apps by using their identifiers.

Get Metadata for Your Books

Fetch metadata for your books by using their identifiers.

Get Metadata for a Catalog App

Fetch metadata for an app from the catalog by using its identifier.

Get Metadata for Multiple Catalog Apps

Fetch metadata for apps from the catalog by using their identifiers.

Get Metadata for a Catalog Book

Fetch metadata for a book from the catalog by using its identifier.

Get Metadata for Multiple Catalog Books

Fetch metadata for books from the catalog by using their identifiers.

Get Catalog Search Results

Fetch metadata for apps and books from the catalog by using a search term.

## See Also

### Essentials

Managing Apps and Books Through Web Services

Associate app and book purchases with users or devices.

Upgrading to the new App and Book Management API

Manage devices and content across your organization using the new API version.

Managing Assets

Retrieve key information to effectively manage assets across an organization’s users and devices.

Managing Users

Retrieve key information to effectively manage users across an organization.

Using Paginated Endpoints

Manage paginated endpoints to efficiently work with large record sets.

Subscribing to Notifications

Listen to notifications to keep track of the latest events for an organization.

Handling Error Responses

Investigate service request errors and troubleshoot solutions.

