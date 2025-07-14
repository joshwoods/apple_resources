

- App Store Connect API
-  List All Customer Reviews for an App 

Web Service Endpoint

# List All Customer Reviews for an App

Get a list of customer reviews for a specific app.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/customerReviews
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the `apps` resource that represents your app. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[customerReviewResponses]`

`[string]`

Fields to return for the included related types.

Possible Values: `responseBody, lastModifiedDate, state, review`

`fields[customerReviews]`

`[string]`

Fields to return for the included related types.

Possible Values: `rating, title, body, reviewerNickname, createdDate, territory, response`

`filter[rating]`

`[string]`

An array of numerical rating values by which to filter. For example, filtering for 1,2,5 shows only reviews with ratings of 1, 2, or 5. The minimum numeric rating value is 1, and the maximum is 5.

`include`

`[string]`

Relationship data to include in the response.

Value: `response`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

`sort`

`[string]`

Attributes by which to sort. Supports one sort parameter at a time.

Possible Values: `rating, -rating, createdDate, -createdDate`

`filter[territory]`

`[string]`

A filter of territories to include in the response.

Possible Values: `ABW, AFG, AGO, AIA, ALB, AND, ANT, ARE, ARG, ARM, ASM, ATG, AUS, AUT, AZE, BDI, BEL, BEN, BES, BFA, BGD, BGR, BHR, BHS, BIH, BLR, BLZ, BMU, BOL, BRA, BRB, BRN, BTN, BWA, CAF, CAN, CHE, CHL, CHN, CIV, CMR, COD, COG, COK, COL, COM, CPV, CRI, CUB, CUW, CXR, CYM, CYP, CZE, DEU, DJI, DMA, DNK, DOM, DZA, ECU, EGY, ERI, ESP, EST, ETH, FIN, FJI, FLK, FRA, FRO, FSM, GAB, GBR, GEO, GGY, GHA, GIB, GIN, GLP, GMB, GNB, GNQ, GRC, GRD, GRL, GTM, GUF, GUM, GUY, HKG, HND, HRV, HTI, HUN, IDN, IMN, IND, IRL, IRQ, ISL, ISR, ITA, JAM, JEY, JOR, JPN, KAZ, KEN, KGZ, KHM, KIR, KNA, KOR, KWT, LAO, LBN, LBR, LBY, LCA, LIE, LKA, LSO, LTU, LUX, LVA, MAC, MAR, MCO, MDA, MDG, MDV, MEX, MHL, MKD, MLI, MLT, MMR, MNE, MNG, MNP, MOZ, MRT, MSR, MTQ, MUS, MWI, MYS, MYT, NAM, NCL, NER, NFK, NGA, NIC, NIU, NLD, NOR, NPL, NRU, NZL, OMN, PAK, PAN, PER, PHL, PLW, PNG, POL, PRI, PRT, PRY, PSE, PYF, QAT, REU, ROU, RUS, RWA, SAU, SEN, SGP, SHN, SLB, SLE, SLV, SMR, SOM, SPM, SRB, SSD, STP, SUR, SVK, SVN, SWE, SWZ, SXM, SYC, TCA, TCD, TGO, THA, TJK, TKM, TLS, TON, TTO, TUN, TUR, TUV, TWN, TZA, UGA, UKR, UMI, URY, USA, UZB, VAT, VCT, VEN, VGB, VIR, VNM, VUT, WLF, WSM, YEM, ZAF, ZMB, ZWE`

`exists[publishedResponse]`

`boolean`

A Boolean value that filters the reviews based on whether the review has a published response in the App Store. Use `true` to return the customer reviews that already have a published response in the App Store. Use `false` to return the customer reviews that don’t have a published response. Note that it’s possible that a review has a response that isn’t yet published.

## Response Codes

` 200 ``OK`

CustomerReviewsResponse

`OK`

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

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

## Discussion

The example below limits the number of reviews returned in the response.

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/apps/682658836/customerReviews?limit=1
```

```
{
  "data": [
    {
      "type": "customerReviews",
      "id": "00000028-b08c-0014-729e-fbd500000000",
      "attributes": {
        "rating": 5,
        "title": "Awesome!!!",
        "body": "It's a really fantastic app!",
        "reviewerNickname": "Anne Johnson",
        "createdDate": "2017-11-15T08:10:34-08:00",
        "territory": "USA"
      },
      "relationships": {
        "response": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/customerReviews/00000028-b08c-0014-729e-fbd500000000/relationships/response",
            "related": "https://api.appstoreconnect.apple.com/v1/customerReviews/00000028-b08c-0014-729e-fbd500000000/response"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/customerReviews/00000028-b08c-0014-729e-fbd500000000"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/apps/682658836/customerReviews?limit=1",
    "next": "https://api.appstoreconnect.apple.com/v1/apps/682658836/customerReviews?cursor=AQ.AMt2C-U&limit=1"
  },
  "meta": {
    "paging": {
      "total": 4326,
      "limit": 1
    }
  }
}
```

