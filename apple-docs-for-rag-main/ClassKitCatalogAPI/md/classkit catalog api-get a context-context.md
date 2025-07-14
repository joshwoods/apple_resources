

- ClassKit Catalog API
-  Get a Context 

Web Service Endpoint

# Get a Context

Fetch information that you previously stored about your app’s assignable activities.

ClassKit 1.0+

## URL

``` source
GET https://classkit-catalog.apple.com/v1/contexts
```

## Query Parameters

`environment`

`string`

 (Required) 

The development or production environment to use for this access. For details, see Testing Your ClassKit Catalog Implementation.

Possible Values: `development, production`

`identifierPath`

`string`

 (Required) 

The identifier path for the context to retrieve. Format this value as a URL-encoded JSON array of strings.

`locale`

`string`

 (Required) 

The locale of the context to retrieve. Use one of the identifiers supported by the Locale structure. It must match a locale that your app supports.

## Response Codes

` 200 ``OK`

ContextsResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

The request contained an error.

` 403 ``Forbidden`

`Forbidden`

The request wasn’t authorized.

## Discussion

### Example

- Request
- Response

```
https://classkit-catalog.apple.com/v1/contexts?environment=development&identifierPath=%5B%22com.apple.www.Quizzer%22%2C%22Quiz%20Catalog%22%2C%22Fun%20Math%20Quiz%22%5D&locale=en-us
```

```
{
  "contexts": [
    {
      "data": {
        "identifierPath": ["com.apple.www.Quizzer", "Quiz Catalog", "Fun Math Quiz"],
        "title": "Fractions Quiz 01",
        "type": "quiz",
        "summary": "This quiz tests your ability to add and subtract fractions.",
        "thumbnailId": "math.png",
        "displayOrder": "1",
        "topic": "math",
        "suggestedAge": ["0", "9223372036854775807"],
        "suggestedCompletionTime": ["0", "0"],
        "isAssignable": true,
        "progressReportingCapabilities": [
          {
            "kind": "score",
            "details": "This reports a student’s score on the quiz."
          },
          {
            "kind": "duration",
            "details": "This tracks the time elapsed on the quiz."
          }
        ]
      },
      "metadata": {
        "locale": "en-us",
        "minimumBundleVersion": "1.0.0",
        "keywords": ["Mathematics", "Fractions", "Quiz", "Grade 5", "Grade 6", "Addition", "Subtraction"],
        "presentableLocales": ["mul"]
      }
    }
  ]
}

```

## See Also

### Declaring Contexts

Preparing Context Data

Adjust how you manage context data when working with the web API.

Create or Replace Contexts

Store information about the assignable content that your educational app provides.

Delete a Context

Remove information that you previously stored about your app’s assignable activities.

object Context

An area of your app that represents an assignable task, like a quiz or a chapter.

object ContextsRequest

A request that you make when modifying context information.

object ContextsResponse

The response you receive after modifying context information.

