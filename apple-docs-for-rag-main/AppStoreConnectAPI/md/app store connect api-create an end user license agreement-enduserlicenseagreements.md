

- App Store Connect API
-  Create an End User License Agreement 

Web Service Endpoint

# Create an End User License Agreement

Add a custom end user license agreement (EULA) to an app and configure the territories to which it applies.

App Store Connect API 1.2+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/endUserLicenseAgreements
```

## HTTP Body

EndUserLicenseAgreementCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

EndUserLicenseAgreementResponse

`Created`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

Use this endpoint to associate a custom license agreement with an app in the specified App Store territories. Any other territories will use the standard Apple-provided license agreement.

In the following example the request contains a blank value for the `agreementText` attribute. Replace that attribute value with your actual agreement text.

### Create a Custom License Agreement for USA and China

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/endUserLicenseAgreements

{
  "data": {
    "type": "endUserLicenseAgreements",
    "attributes": {
      "agreementText": "..."
    },
    "relationships": {
      "app": {
        "data": {
          "type": "apps",
          "id": "284993459"
        }
      },
      "territories": {
        "data": [
          {
            "type": "territories",
            "id": "USA"
          },
          {
            "type": "territories",
            "id": "CHN"
          }
        ]
      }
    }
  }
}
```

```
{
  "data" : {
    "type" : "endUserLicenseAgreements",
    "id" : "b25d1669-d6b1-4e9b-8679-02863557222a",
    "attributes" : {
      "agreementText" : "..."
    },
    "relationships" : {
      "app" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/endUserLicenseAgreements/b25d1669-d6b1-4e9b-8679-02863557222a/relationships/app",
          "related" : "https://api.appstoreconnect.apple.com/v1/endUserLicenseAgreements/b25d1669-d6b1-4e9b-8679-02863557222a/app"
        }
      },
      "territories" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/endUserLicenseAgreements/b25d1669-d6b1-4e9b-8679-02863557222a/relationships/territories",
          "related" : "https://api.appstoreconnect.apple.com/v1/endUserLicenseAgreements/b25d1669-d6b1-4e9b-8679-02863557222a/territories"
        }
      }
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/endUserLicenseAgreements/b25d1669-d6b1-4e9b-8679-02863557222a"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/endUserLicenseAgreements"
  }
}
```

## See Also

### Creating, Modifying, and Deleting an EULA

Modify an End User License Agreement

Update the text or territories for your custom end user license agreement.

Delete an End User License Agreement

Delete the custom end user license agreement that is associated with an app.

