

- Swift
- Sequence
-  smallestSubset(groupedBy:) 

Instance Method

# smallestSubset(groupedBy:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func smallestSubset(groupedBy keyPath: KeyPath) -> [Self.Element] where DonationInfo : Decodable, DonationInfo : Encodable, DonationInfo : Sendable, Value : Hashable, Self.Element == Tips.Event.Donation
```

