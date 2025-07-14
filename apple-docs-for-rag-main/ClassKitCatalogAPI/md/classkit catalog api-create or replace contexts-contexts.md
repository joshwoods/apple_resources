

- ClassKit Catalog API
-  Create or Replace Contexts 

Web Service Endpoint

# Create or Replace Contexts

Store information about the assignable content that your educational app provides.

ClassKit 1.0+

## URL

``` source
POST https://classkit-catalog.apple.com/v1/contexts
```

## Query Parameters

`environment`

`string`

 (Required) 

The development or production environment to use for this access. For details, see Testing Your ClassKit Catalog Implementation.

Possible Values: `development, production`

## HTTP Body

ContextsRequest

The context or contexts to add.

Content-Type: application/json

## Response Codes

` 201 ``Created`

`Created`

The request succeeded.

` 202 ``Accepted`

`Accepted`

The API accepted but hasn’t completed the request. To ask for a status update later, see Get Status.

` 400 ``Bad Request`

`Bad Request`

The request contained an error.

` 403 ``Forbidden`

`Forbidden`

The request wasn’t authorized.

## Discussion

Define parent contexts of any of the contexts defined in this call, either in a previous call to the same endpoint, or as part of the same call.

You can specify up to 200 contexts for any one call to this endpoint. The call overwrites any contexts that already exist with the same identifier path and locale.

### Example

- Request
- Response

```
{
  "contexts": [
    {
      "metadata": {
        "locale": "en-us",
        "minimumBundleVersion": "1.0.0",
        "keywords": [
          "Mathematics",
          "Fractions",
          "Quiz",
          "Grade 5",
          "Grade 6",
          "Addition",
          "Subtraction"
        ],
        "presentableLocales": [
          "mul"
        ]
      },
      "data": {
        "identifierPath": [
          "com.apple.www.Quizzer",
          "Quiz Catalog",
          "Fun Math Quiz"
        ],
        "title": "Fractions Quiz 01",
        "type": "quiz",
        "summary": "This quiz tests your ability to add and subtract fractions.",
        "thumbnailId": "math.png",
        "displayOrder": "1",
        "topic": "math",
        "suggestedAge": [
          0,
          9223372036854775807
        ],
        "suggestedCompletionTime": [
          0,
          0
        ],
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
      }
    },
    {
      "metadata": {
        "locale": "es-us",
        "minimumBundleVersion": "1.0.0",
        "keywords": [
          "Matemáticas",
          "Fracciones",
          "Examen",
          "Grado 5",
          "Grado 6",
          "Adición",
          "Sustracción"
        ],
        "presentableLocales": [
          "es-us"
        ]
      },
      "data": {
        "identifierPath": [
          "com.apple.www.Quizzer",
          "Quiz Catalog",
          "Fun Math Quiz"
        ],
        "title": "Quiz Fracciones 01",
        "type": "quiz",
        "summary": "Este cuestionario evaluará su capacidad para sumar y restar fracciones.",
        "thumbnailId": "math.png",
        "displayOrder": "1",
        "topic": "math",
        "suggestedAge": [
          0,
          9223372036854775807
        ],
        "suggestedCompletionTime": [
          0,
          0
        ],
        "isAssignable": true,
        "progressReportingCapabilities": [
          {
            "kind": "score",
            "details": "Esto informa el puntaje de un estudiante en el cuestionario."
          },
          {
            "kind": "duration",
            "details": "Esto rastrea el tiempo transcurrido en la prueba."
          }
        ]
      }
    },
    {
      "metadata": {
        "locale": "en-us",
        "presentableLocales": [
          "mul"
        ]
      },
      "data": {
        "identifierPath": [
          "com.apple.www.Quizzer",
          "Quiz Catalog"
        ],
        "title": "Quiz Catalog",
        "type": "section",
        "summary": "This is a catalog of quizzes for you to complete.",
        "thumbnailId": "catalog.png",
        "displayOrder": "1"
      }
    },
    {
      "metadata": {
        "locale": "es-us",
        "presentableLocales": [
          "es-us"
        ]
      },
      "data": {
        "identifierPath": [
          "com.apple.www.Quizzer",
          "Quiz Catalog"
        ],
        "title": "Catálogo de Cuestionarios",
        "type": "section",
        "summary": "Este es un catálogo de cuestionarios para completar.",
        "thumbnailId": "catalog.png",
        "displayOrder": "1"
      }
    },
    {
      "metadata": {
        "locale": "es-us"
      },
      "data": {
        "identifierPath": [
          "com.apple.www.Quizzer"
        ],
        "title": "Quizzer",
        "type": "app"
      }
    },
    {
      "metadata": {
        "locale": "en-us",
        "presentableLocales": [
          "mul"
        ]
      },
      "data": {
        "identifierPath": [
          "com.apple.www.Quizzer"
        ],
        "title": "Quizzer",
        "type": "app"
      }
    }
  ]
}
```

```
```

## See Also

### Declaring Contexts

Preparing Context Data

Adjust how you manage context data when working with the web API.

Get a Context

Fetch information that you previously stored about your app’s assignable activities.

Delete a Context

Remove information that you previously stored about your app’s assignable activities.

object Context

An area of your app that represents an assignable task, like a quiz or a chapter.

object ContextsRequest

A request that you make when modifying context information.

object ContextsResponse

The response you receive after modifying context information.

