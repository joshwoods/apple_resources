

- Apple Search Ads
-  Get Supported Countries or Regions 

Web Service Endpoint

# Get Supported Countries or Regions

Fetches supported languages and language codes.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/countries-or-regions
```

## Query Parameters

`countriesOrRegions`

`string`

Filters by ISO alpha-2 country codes using one or more comma-separated values. For example, use `https://api.searchads.apple.com/api/v5/countries-or-regions?countriesOrRegions=US` for a single country or region, or `https://api.searchads.apple.com/api/v5/countries-or-regions?countriesOrRegions=US,` `MX` for multiple countries or regions.

## Response Codes

` 200 ``OK`

CountriesOrRegionsListResponse

`OK`

If the call succeeds, the API returns the CountriesOrRegionsListResponse object in the response payload with an HTTP status code of `200(OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

Content-Type: application/json

` 400 ``Bad Request`

ApiErrorResponse

`Bad Request`

An invalid query or missing required parameters.

Content-Type: application/json

` 401 ``Unauthorized`

ApiErrorResponse

`Unauthorized`

An unauthenticated call fails to get the requested response.

Content-Type: application/json

` 403 ``Forbidden`

ApiErrorResponse

`Forbidden`

Insufficient rights to the resource.

Content-Type: application/json

` 429 `

ApiErrorResponse

The API calls exceed rate-limit thresholds. See the Rate Limits subsection of Calling the Apple Search Ads API.

Content-Type: application/json

` 500 ``Internal Server Error`

ApiErrorResponse

`Internal Server Error`

The Apple Search Ads server is temporarily down or unreachable. The request may be valid, but you need to retry it later.

Content-Type: application/json

## Mentioned in 

Apple Search Ads Campaign Management API 4

## Discussion

Use this endpoint to fetch supported product page languages for countries or regions.

### Payload example 1: Get supported countries or regions

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/countries-or-regions?countriesOrRegions=US,AU,GB,CA
```

```
{
   "data": [
        {
            "countryOrRegion": “US”,
            "supportedLanguages": [
                {
                    "language": "en",
                    "languageCode": "en-US"
                },
                {
                    "language": “es”,
                    "languageCode": "es-MX"
                }
            ],
            "defaultLanguage": {
                "language": "en",
                "languageCode": "en-US"
            }
        },
        {
            "countryOrRegion": "AU",
            "supportedLanguages": [
                {
                    "language": "en",
                    "languageCode": "en-AU"
                },
                {
                    "language": "en",
                    "languageCode": "en-GB"
                }
            ],
            "defaultLanguage": {
                "language": "en",
                "languageCode": "en-AU"
            }
        },
        {
            "countryOrRegion": "GB",
            "supportedLanguages": [
                {
                    "language": "en",
                    "languageCode": "en-GB"
                }
            ],
            "defaultLanguage": {
                "language": "en",
                "languageCode": "en-GB"
            }
        },
        {
            "countryOrRegion": "CA",
            "supportedLanguages": [
                {
                    "language": "en",
                    "languageCode": "en-CA"
                },
                {
                    "language”: "fr",
                    "languageCode": "fr-CA"
                }
            ],
            "defaultLanguage": {
                "language": "en",
                "languageCode": "en-CA"
            }
        }
    ]
}
```

### Payload example 2: Get supported countries or regions

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/countries-or-regions?countriesOrRegions=CA
```

```
{
  "countryOrRegion": "CA",
  "supportedLocales": [
    {
      "language": "en",
      "languageCode": "en-CA"
    },
    {
      "language": "fr",
      "languageCode": "fr-CA"
    }
  ],
  "defaultLanguages": [
    {
      "language": "en",
      "languageCode": "en-CA"
    },
    {
      "language": "fr",
      "languageCode": "fr-CA"
    }
  ]
}
```

## See Also

### Product Page Endpoints

Get Product Pages

Fetches metadata of all your custom product pages.

Get Product Pages by Identifier

Fetches metadata for a specific product page.

Get Product Page Locales

Fetches product page locales by identifier.

Get App Preview Device Sizes

Fetches supported app preview device-size mappings.

