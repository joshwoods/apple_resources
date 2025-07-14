

- Foundation
- URLResourceKey
-  volumeAvailableCapacityForImportantUsageKey 

Type Property

# volumeAvailableCapacityForImportantUsageKey

Key for the volume’s available capacity in bytes for storing important resources (read-only).

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
static let volumeAvailableCapacityForImportantUsageKey: URLResourceKey
```

## Mentioned in 

Checking Volume Storage Capacity

## Discussion

Important

This API has the potential of being misused to access device signals to try to identify the device or user, also known as fingerprinting. Regardless of whether a user gives your app permission to track, fingerprinting is not allowed. When you use this API in your app or third-party SDK (an SDK not provided by Apple), declare your usage and the reason for using the API in your app or third-party SDK’s `PrivacyInfo.xcprivacy` file. For more information, including the list of valid reasons for using the API, see Describing use of required reason API.

## See Also

### Volume capacity keys

Checking Volume Storage Capacity

Confirm that you have enough local storage space for a large amount of data.

static let volumeAvailableCapacityKey: URLResourceKey

Key for the volume’s available capacity in bytes (read-only).

static let volumeAvailableCapacityForOpportunisticUsageKey: URLResourceKey

Key for the volume’s available capacity in bytes for storing nonessential resources (read-only).

static let volumeTotalCapacityKey: URLResourceKey

Key for the volume’s total capacity in bytes (read-only).

