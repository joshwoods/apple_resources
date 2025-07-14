

- Apple News
- Apple News API
-  Apple News API Release Notes for iOS 17, iPadOS 17, and macOS 14 

Article

# Apple News API Release Notes for iOS 17, iPadOS 17, and macOS 14

Learn about the new features and deprecated fields in Apple News API.

## Overview

These features were added in the latest Apple News API release:

- The Create an Article endpoint throws a 400 error if you attempt to publish an article with a publication date before 1970, and a warning if the publication date is before 2015.

- The Update an Article endpoint throws a 400 error if you attempt to update an article with a publication date before 1970, and a warning if the publication date is before 2015.

These features were added in a previous Apple News API release:

- The Search Articles in a Channel endpoint throws a 429 error if you exceed the number of articles that you can search for in a channel within a specific time window.

- The Search Articles in a Section endpoint throws a 429 error if you exceed the number of articles that you can search for in a section within a specific time window.

- The Update an Article endpoint throws a 429 error if you exceed the number of articles that you can update within a specific time window.

- The Read Article Information endpoint throws a warning message for an optimized article.

- The Update an Article endpoint throws a 202 error if you attempt to update an optimized article.

- The Delete an Article endpoint throws a 400 error if you attempt to delete an optimized article.

This field is no longer supported in Apple News API:

- `accessoryText` is deprecated in Create Article Metadata Fields and Update Article Metadata Fields. Use the `authors` property in the Apple News Format Metadata object instead.

