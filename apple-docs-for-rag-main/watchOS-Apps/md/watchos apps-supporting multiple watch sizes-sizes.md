

- watchOS apps
-  Supporting multiple watch sizes 

Article

# Supporting multiple watch sizes

Customize the layout of your user interface to support all Apple Watch sizes.

## Overview

With the addition of Apple Watch Series 10, watchOS apps now support seven watch sizes.

| Devices                            | Sizes           |
|------------------------------------|-----------------|
| Apple Watch Series 4, 5, 6, and SE | 40 mm and 44 mm |
| Apple Watch Series 7, 8, and 9     | 41 mm and 45 mm |
| Apple Watch Series 10              | 42 mm and 46 mm |
| Apple Watch Ultra                  | 49 mm           |

In addition to adding two new sizes, Apple Watch Series 10 also has a slightly different aspect ratio–gaining a bit more width. It also has rounder corners.

When Apple Watch Series 10 runs an app compiled for watchOS 10 or earlier, the system letterboxes the interface, centering it on the screen. Additionally, the Series 10 clips the corners of the letter-boxed content; however, it doesn’t clip the safe area. To fully use the Series 10 sizes, build your app with the watchOS 11 SDK or later.

### Create a dynamic layout

When designing your app, be sure to consider all available watch sizes. Where possible, use resizable objects to fill the available space. Resizable objects help create flexible layouts and minimize the amount of customization you need to support for the different sizes. If necessary, you can customize your layout for specific sizes; however, when creating the layout for larger screens, use the additional space to display larger controls and assets, rather than filling the screen with additional controls.

For additional design information, see Designing for watchOS.

### Use safe areas and scene padding

Most watches have rounded corners that may clip scrolling content. Some also bend content around the bevel, which can affect the appearance of anything placed near the sides. Finally, each screen keeps a margin between the text in its status and notification bars, and the edge of the screen. When laying out your content, you typically align text with the leading edge of the navigation bar’s title or the back button, and the trailing edge of the status bar’s text.

The system provides the following tools to help you manage your content:

Safe area insets  
Defines the area on the screen where you can safely display content. The safe area is the region below the status bar that avoids the rounded corners.

Scene padding  
Provides the same leading and trailing margin as the navigation and status bars. This padding also ensures that the watch’s bevel doesn’t distort the content.

The following figures show the safe area and scene padding for all watch sizes. The *h* value at the top is the number of points from the top of the safe area to the bottom of the status bar. The *y* distance indicates the size of the text margin.

- Series 4, 5, 6, and SE (40mm and 44mm)
- Series 7, 8, and 9 (41mm and 45mm)
- Series 10 (42mm and 46mm)
- Ultra (49mm)

By default, SwiftUI views fill the safe area. Scrolling content, such as a list view, automatically settles within the safe areas. To disable the safe area, use the ignoresSafeArea(_:edges:) view modifier.

To align items with the status and navigation bar, call scenePadding(_:) on the view. In general, align text with the status and navigation bar. In watchOS 11 and later, Button automatically aligns to the text margins. The rounded rectangle for a List horizontally fills the safe area, but its content aligns with the status and navigation bar.

```
@State var showing = true

var body: some View {
    Text("Hello World")
    // Displaying a sheet ensures that there are items on both sides
    // of the status bar.
        .sheet(isPresented: $showing) {
            VStack {

                Spacer()

                // Align the text with the status bar.
                Text("The quick brown fox jumps over the lazy dog.")
                    .scenePadding(.horizontal)

                Spacer()

                // The button automatically aligns with the status bar.
                Button("My Button") {
                    print("Button Pressed!")
                }
            }
        }
}
```

 For additional design information, see Layout.

### Support dynamic type

Use dynamic type so the wearer can modify the size of text components in your app. Dynamic type helps users who need larger text for better readability. It also accommodates those who can read smaller text, allowing more information to appear on the screen. Apps that support Dynamic Type provide an experience that is consistent with the system apps. For more information, see Applying custom fonts to text.

Different watch sizes use different default dynamic type sizes.

| Device                         | Dynamic type size |
|--------------------------------|-------------------|
| 40 mm, 41 mm, and 42 mm        | Large             |
| 44 mm, 45 mm, 46 mm, and 49 mm | XLarge            |

Note

The wearer can change the dynamic type size, including using accessibility sizes. Always check your app’s appearance with all available type sizes.

For additional design information, see Typography.

### Manage assets

To provide an asset that adapts to all watch sizes, create a scalable PDF asset. Add a PDF to the asset catalog as a 2x image asset, then set its Auto Scaling attribute to Automatic.

When you load the PDF, the system scales the image based on the current device’s size as listed in the table.

| Watch Size        | Image Scale |
|-------------------|-------------|
| 38 mm             | 90%         |
| 40 mm             | 100%        |
| 41 mm             | 106%        |
| 42 mm (Series 3)  | 100%        |
| 42 mm (Series 10) | 106%        |
| 44 mm             | 110%        |
| 45 mm             | 119%        |
| 46 mm             | 119%        |
| 49 mm             | 119%        |

For more design information, see Images.

### Preview multiple sizes

When designing a watchOS app, you can use Xcode previews to check your app’s layout. You can display one or more previews using the `#Preview` macro.

```
#Preview {
    ContentView()
}
```

You can then use the Preview destination picker to switch between different devices.

You can also view all the dynamic type sizes for that device by selecting the Dynamic Type Variants option.

For more information, see Previewing your app’s interface in Xcode.

## See Also

### User interface

Building a productivity app for Apple Watch

Create a watch app to manage and share a task list and visualize the status with a chart.

Designing your app for the Always On state

Customize your watchOS app’s user interface for continuous display.

Setting the app’s accent color

Set your app’s accent color.

