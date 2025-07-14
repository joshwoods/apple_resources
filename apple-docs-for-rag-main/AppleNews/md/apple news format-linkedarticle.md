

- Apple News Format
-  LinkedArticle 

Object

# LinkedArticle

A relationship between your article and another Apple News article.

Apple News Format 1.7+

``` source
object LinkedArticle
```

## Properties

`relationship`

`string`

 (Required) 

The type of relationship between the article and the linked document.

Valid values:

- `related`. The linked article is an article on the same topic, part of the same dossier, or provides more information about the subjects discussed.

- `promoted`. The linked article isn’t directly related, but deserves additional promotion because the article covers another important topic. This value also puts the article at the top of the channel feed.

Possible Values: `related, promoted`

`URL`

`uri`

 (Required) 

The URL for the link, which can be either an Apple News link, like `https://apple.news/[article_id]`, or a link to an article on your website, if the website link matches the `canonicalURL` metadata property of the linked article. For more information about `canonicalURL`, see Metadata.

## Discussion

You can control lists of links that people see in articles by using the `links` array in Metadata. If you are linking to a sponsored article, ensure that the Create an Article request uses the `isSponsored` flag.

### Example

```
{
  "metadata": {
    "excerpt": "This is a sample sports article.",
    "thumbnailURL": "bundle://Football.jpg",
    "datePublished": "2018-09-09T14:45:45+00:00",
    "dateCreated": "2018-09-08T12:41:00+00:00",
    "dateModified": "2018-09-10T12:41:00+00:00",
    "authors": [
      "Anne Johnson"
    ],
    "campaignData": {
      "sport": [
        "football"
      ],
      "event": [
        "Football"
      ],
      "author": [
        "John Appleseed"
      ]
    },
    "generatorName": "Generator",
    "generatorVersion": "1.0",
    "canonicalURL": "https://example.com/articles/2015/original-article.html",
    "links": [
      {
        "URL": "https://apple.news/AT6kNQslCQy6EE4bF8hpOoQ",
        "relationship": "related"
      }
    ]
  }
}
```

## See Also

### Article Metadata

object Metadata

Information about your article, including author name, creation date, publication date, keywords, and excerpt.

object Issue

The object for defining information about an issue.

