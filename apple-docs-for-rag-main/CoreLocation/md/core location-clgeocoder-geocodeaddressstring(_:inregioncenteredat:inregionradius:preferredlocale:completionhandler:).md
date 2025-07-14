

- Core Location
- CLGeocoder
-  geocodeAddressString(\_:inRegionCenteredAt:inRegionRadius:preferredLocale:completionHandler:) 

Instance Method

# geocodeAddressString(\_:inRegionCenteredAt:inRegionRadius:preferredLocale:completionHandler:)

visionOS 1.0+

``` source
func geocodeAddressString(
    _ addressString: String,
    inRegionCenteredAt centroid: CLLocationCoordinate2D,
    inRegionRadius radius: CLLocationDistance,
    preferredLocale locale: Locale?,
    completionHandler: @escaping CLGeocodeCompletionHandler
)
```

``` source
func geocodeAddressString(
    _ addressString: String,
    inRegionCenteredAt centroid: CLLocationCoordinate2D,
    inRegionRadius radius: CLLocationDistance,
    preferredLocale locale: Locale?
) async throws -> [CLPlacemark]
```

