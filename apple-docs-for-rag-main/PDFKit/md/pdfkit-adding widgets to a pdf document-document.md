

- PDFKit
-  Adding Widgets to a PDF Document 

Article

# Adding Widgets to a PDF Document

Add text, button, and choice widgets to a PDF document.

## Overview

Widgets are interactive form elements that you can add to a PDF to make it easier to enter and submit information. Widgets are a special annotation subtype. To learn more about non-interactive custom annotations, see Adding Custom Graphics to a PDF.

Each widget type has several variations. A button can be a radio button, a check box, or a push button. A choice widget can be a list box, which is a table of options, or a combo box, which is like a dropdown.

### Create a Widget Annotation

Create a PDF annotation of type widget. This example initializes a widget annotation with rectangular bounds:

```
let radioButton = PDFAnnotation(bounds: CGRect(x: 135, y: 200, width: 24, height: 24), forType: .widget, withProperties: nil)
```

### Specify a Field Type and a Control Type

Specify a widgetFieldType that is a PDFAnnotationWidgetSubtype. The three different subtypes are text, button, and choice. Here you will create a button widget for the radio button:

```
radioButton.widgetFieldType = .button

```

Set the widget control type. For a button widget, there are three possible control types: PDFWidgetControlType.radioButtonControl, PDFWidgetControlType.checkBoxControl, and PDFWidgetControlType.pushButtonControl.

```
radioButton.widgetControlType = .radioButtonControl

```

### Adjust Widget Properties

Adjust properties to highlight the widget so it is more visible. The following example adds a blue background to a radio button widget.

```
radioButton.backgroundColor = UIColor.blue

```

Properties will be different depending on the field type. If you have multiple radio buttons and want to group them together, specify the same fieldName property. Specify different buttonWidgetStateString properties for each button if you should only select one at a time. For a text field, you can use widgetStringValue to specify placeholder text and font to specify the font of the field’s text.

### Add the Annotation to Your PDF

Add the annotation to the page.

```
page.addAnnotation(radioButton)

```

You can combine many different kinds of widgets on your PDF. Using a combination of widgets can help you turn a PDF document into an interactive form. For more details on widget options, see PDFAnnotation.

## See Also

### Annotations

Adding Custom Graphics to a PDF

Create and add custom annotation and page graphics to your PDF document.

Custom Graphics

Demonstrates adding a watermark to a PDF page.

PDF Widgets

Demonstrates adding widgets—interactive form elements—to a PDF document.

class PDFAnnotation

An annotation in a PDF document.

