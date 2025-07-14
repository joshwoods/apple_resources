

- SensorKit
- SRDeviceUsageReport
-  SRDeviceUsageReport.CategoryKey 

Structure

# SRDeviceUsageReport.CategoryKey

Categories of apps or websites that the user uses.

``` source
struct CategoryKey
```

## Topics

### Initializers

init(rawValue: String)

Creates a new category.

### Categories

static let books: SRDeviceUsageReport.CategoryKey

An app category for reading books.

static let business: SRDeviceUsageReport.CategoryKey

An app category for doing business.

static let catalogs: SRDeviceUsageReport.CategoryKey

An app category for reading catalogs.

static let developerTools: SRDeviceUsageReport.CategoryKey

An app category for creating apps.

static let education: SRDeviceUsageReport.CategoryKey

An app category for learning.

static let entertainment: SRDeviceUsageReport.CategoryKey

An app category for entertainment.

static let finance: SRDeviceUsageReport.CategoryKey

An app category for finance.

static let foodAndDrink: SRDeviceUsageReport.CategoryKey

An app category for dining.

static let games: SRDeviceUsageReport.CategoryKey

An app category for gaming.

static let graphicsAndDesign: SRDeviceUsageReport.CategoryKey

An app category for graphic design.

static let healthAndFitness: SRDeviceUsageReport.CategoryKey

An app category for health and fitness.

static let kids: SRDeviceUsageReport.CategoryKey

An app category for children.

static let lifestyle: SRDeviceUsageReport.CategoryKey

An app category for lifestyle.

static let medical: SRDeviceUsageReport.CategoryKey

An app category for healthcare.

static let miscellaneous: SRDeviceUsageReport.CategoryKey

An app category for miscellaneous apps.

static let music: SRDeviceUsageReport.CategoryKey

An app category for music.

static let navigation: SRDeviceUsageReport.CategoryKey

An app category for navigation.

static let news: SRDeviceUsageReport.CategoryKey

An app category for news.

static let newsstand: SRDeviceUsageReport.CategoryKey

An app category for Apple News.

static let photoAndVideo: SRDeviceUsageReport.CategoryKey

An app category for photography and film.

static let productivity: SRDeviceUsageReport.CategoryKey

An app category for productivity.

static let reference: SRDeviceUsageReport.CategoryKey

An app category for reference.

static let shopping: SRDeviceUsageReport.CategoryKey

An app category for shopping.

static let socialNetworking: SRDeviceUsageReport.CategoryKey

An app category for social networking.

static let sports: SRDeviceUsageReport.CategoryKey

An app category for sports.

static let stickers: SRDeviceUsageReport.CategoryKey

An app category for stickers.

static let travel: SRDeviceUsageReport.CategoryKey

An app category for travel.

static let utilities: SRDeviceUsageReport.CategoryKey

An app category for utilities.

static let weather: SRDeviceUsageReport.CategoryKey

An app category for weather.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Analyzing App Use

var applicationUsageByCategory: [SRDeviceUsageReport.CategoryKey : [SRDeviceUsageReport.ApplicationUsage]]

The usage time of apps per category.

class ApplicationUsage

An object that describes the user’s app activity over a period of time.

