

- Apple News
- Apple News API
-  Formatting Strings 

Article

# Formatting Strings

Learn how to format strings to pass to the API client.

## Overview

When using command-line utilities to pass a string to the API client, enclose the string in single quotation marks to treat the text literally. When you enclose a string in double quotation marks, you need to escape certain ASCII characters (for example, the \$ character).

This example uses single quotation marks:

```
alert-body='Big Company is acquiring Smaller Company for $2.5 billion.'
```

This example shows the result of using single quotation marks:

```
"alertBody": "Big Company is acquiring Smaller Company for $2.5 billion."
```

This example uses double quotation marks incorrectly:

```
alert-body="Big Company is acquiring Smaller Company for $2.5 billion."
```

This example shows the result of using double quotation marks incorrectly. A string in double quotation marks with the \$ sign should include an escape character:

```
"alertBody": "Big Company is acquiring Smaller Company for .5 billion."
```

This example correctly uses double quotation marks with an escape character:

```
alert-body="Big Company is acquiring Smaller Company for \$2.5 billion."
```

This example shows the result of using double quotation marks with an escape character:

```
"alertBody": "Big Company is acquiring Smaller Company for $2.5 billion."
```

## See Also

### Essentials

Getting Ready to Publish and Manage Your Articles

Get set up for using the Apple News API.

About the Apple News Security Model

Learn how the Apple News API authenticates clients, authorizes your news channel, and enforces confidentiality.

About Apple News API Field Types

Understand the standard field types used in the Apple News API.

