---
type: function(pointInfo)
---
---
##### shortDescription
Allows you to change the appearance of specific tooltips.

##### param(pointInfo): object
Defines the point that is currently hovered over.

##### return: object
The text or markup to be displayed in a tooltip, along with that tooltip's settings.

---
This option should be assigned a function returning a specific object. The following fields can be specified in this object.

- **color**		
Specifies the [color](/api-reference/20%20Data%20Visualization%20Widgets/BaseWidget/1%20Configuration/tooltip/color.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxPieChart/Configuration/tooltip/#color') of a tooltip.

- **text**		
Specifies the text displayed by a tooltip.

- **html**		
Specifies the HTML markup displayed by a tooltip.
[note]If you are going to use external resources (for example, images) in the markup, specify the size of the area they will occupy beforehand.

- **fontColor**		
Specifies the color of the text displayed by a tooltip.

- **borderColor**		
Specifies the color of the tooltip border.

When implementing the function for this option, you can use information about the tooltip's point. For example, you can access the argument or value of this point. To do this, use the following fields of the **this** object.

* **value**   
Specifies the value of the currently hovered point.
* **valueText**   
Specifies the value of the currently hovered point with applied formatting if the **format** property is specified.
* **argument**   
Specifies the argument value of the currently hovered point.
* **argumentText**   
Specifies the argument value of the currently hovered point with applied formatting if the **argumentFormat** property is specified.
* **percent**     
Specifies the percent value of the currently hovered point.
* **percentText**    
Specifies the percent value of the currently hovered point with **percentPrecision** (optional) applied.
* **point**    
Provides access to the hovered point. To learn more about the field and methods of the point object, refer to the [Point](/api-reference/20%20Data%20Visualization%20Widgets/15%20dxPieChart/7%20Chart%20Elements '/Documentation/ApiReference/Data_Visualization_Widgets/dxPieChart/Chart_Elements/') topic in the "Chart Elements" reference section.

The function's parameter represents the same object as the **this** object. If appropriate, you can use the function's parameter to obtain the value that is currently represented by a tooltip.

To get general information on data formatting, refer to the [Data Formatting](/concepts/20%20Data%20Visualization/40%20Common/30%20Data%20Formatting '/Documentation/Guide/Data_Visualization/Common/Data_Formatting/') topic.

<a href="http://js.devexpress.com/Demos/WidgetsGallery/#demo/chartschartsadvancedfeaturestooltiphtmlsupport" class="button orange small fix-width-155" style="margin-right: 20px;" target="_blank">View Demo</a>