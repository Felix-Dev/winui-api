---
-api-id: P:Microsoft.UI.Xaml.Controls.TreeView.ItemContainerStyleSelector
-api-type: winrt property

---
<!-- Property syntax.
public StyleSelector ItemContainerStyleSelector { get;  set; }
-->

# Microsoft.UI.Xaml.Controls.TreeView.ItemContainerStyleSelector


## -description

Gets or sets a reference to a custom [StyleSelector](styleselector.md) logic class. The [StyleSelector](styleselector.md) returns different [Style](../windows.ui.xaml/style.md) values to use for the item container based on characteristics of the object being displayed.


## -property-value

A custom [StyleSelector](styleselector.md) logic class.


## -remarks


## -see-also


## -examples


## -xaml-syntax

```xaml
<TreeView ItemContainerStyleSelector="styleSelectorReference" />
```


## -xaml-values

<dl><dt>styleSelectorReference</dt><dd>styleSelectorReferenceA reference to an existing StyleSelector. Typically this is a keyed resource, which you reference through a {StaticResource} markup extension usage.</dd>
</dl>


