

- Device Management
-  Update the eSIM Cellular Plan 

Web Service Endpoint

# Update the eSIM Cellular Plan

Query a carrier URL for active eSIM cellular-plan profiles on a device.

iOS 13.0+iPadOS 13.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#RefreshCellularPlansCommand
```

## HTTP Body

RefreshCellularPlansCommand

The command to query a carrier URL for active eSIM cellular-plan profiles.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

RefreshCellularPlansResponse

`OK`

A response from the device after it processes the command to query a carrier URL for active eSIM cellular-plan profiles.

Content-Type: application/xml

## Discussion

This command is supported on iPad with iPadOS 13 and later and on iPhone with iOS 14 and later.

### Command Availability

|                            |                  |
|----------------------------|------------------|
| Device Channel             | iOS, Shared iPad |
| User Channel               | \-               |
| Requires Supervision       | \-               |
| Allowed in User Enrollment | \-               |
| Required Access Right      | \-               |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        RefreshCellularPlans
        eSIMServerURL
        http://example.server.com

    CommandUUID
    0001_RefreshCellularPlans

```

```

    CommandUUID
    0001_RefreshCellularPlans
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object RefreshCellularPlansCommand

The command to query a carrier URL for active eSIM cellular-plan profiles.

object RefreshCellularPlansResponse

A response from the device after it processes the command to query a carrier URL for active eSIM cellular-plan profiles.

