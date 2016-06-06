<properties
    pageTitle="Pie chart control: reference | Microsoft PowerApps"
    description="Information, including properties and examples, about the Pie chart control"
    services=""
    suite="powerapps"
    documentationCenter="na"
    authors="aftowen"
    manager="erikre"
    editor=""
    tags=""/>

<tags
   ms.service="powerapps"
   ms.devlang="na"
   ms.topic="article"
   ms.tgt_pltfrm="na"
   ms.workload="na"
   ms.date="03/11/2016"
   ms.author="anneta"/>

# Pie chart control in PowerApps #
A control that shows relative values in comparison to each other.

## Description ##
Add a **Pie chart** control if you want to show relative data from a table that contains labels in the leftmost column and values in the second column from the left.

## Key properties ##

**[Items](properties-core.md)** – The source of data that appears in a control such as a gallery, a list, or a chart.

**ShowLabels** – Whether a pie chart shows the value that's associated with each of its wedges.

## Additional properties ##

**[BorderColor](properties-color-border.md)** – The color of a control's border.

**[BorderStyle](properties-color-border.md)** – Whether a control's border is **Solid**, **Dashed**, **Dotted**, or **None**.

**[BorderThickness](properties-color-border.md)** – The thickness of a control's border.

**[Color](properties-color-border.md)** – The color of text in a control.

**[Disabled](properties-core.md)** – Whether the user can interact with the control.

**[DisabledBorderColor](properties-color-border.md)** – The color of a control's border if the control's **[Disabled](properties-core.md)** property is set to **true**.

**Explode** – The distance between wedges in a pie chart.

**[Font](properties-text.md)** – The name of the family of fonts in which text appears.

**[Height](properties-size-location.md)** – The distance between a control's top and bottom edges.

**[HoverBorderColor](properties-color-border.md)** – The color of a control's border when the user keeps the mouse pointer on that control.

**ItemBorderColor** – The color of the border around each wedge in a pie chart.

**ItemBorderThickness** – The thickness of the border around each wedge in a pie chart.

**ItemColorSet** – The color of each data point in a chart.

**LabelPosition** – The location of labels in a pie chart relative to its wedges.

**[OnSelect](properties-core.md)** – How the app responds when the user taps or clicks a control.

**[PressedBorderColor](properties-color-border.md)** – The color of a control's border when the user taps or clicks that control.

**[Size](properties-text.md)** – The font size of the text that appears on a control.

**[Visible](properties-core.md)** – Whether a control appears or is hidden.

**[Width](properties-size-location.md)** – The distance between a control's left and right edges.

**[X](properties-size-location.md)** – The distance between the left edge of a control and the left edge of the screen.

**[Y](properties-size-location.md)** – The distance between the top edge of a control and the top edge of the screen.

## Related functions ##

[**Max**( *DataSource*, *ColumnName* )](../functions/function-aggregates.md)

## Example ##
1. Add a **[Button](control-button.md)** control, and set its **[OnSelect](properties-core.md)** property to this formula:<br>
**Collect(Revenue2015, {Product:"Europa", Revenue:27000}, {Product:"Ganymede", Revenue:26300}, {Product:"Callisto", Revenue:29200})**

	Don't know how to [add and configure a control](../add-configure-controls.md)?

	Want more information about the **[Collect](../functions/function-clear-collect-clearcollect.md)** function or [other functions](../formula-reference.md)?

1. Press F5, click or tap the **[Button](control-button.md)** control, and then press Esc to return to the default workspace.

1. Add a **Pie chart** control, and set its **[Items](properties-core.md)** property to **Revenue2015**.

	The **Pie chart** control shows revenue data for each product in relation to the other products.