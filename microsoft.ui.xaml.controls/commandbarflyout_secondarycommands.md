---
-api-id: P:Microsoft.UI.Xaml.Controls.CommandBarFlyout.SecondaryCommands
-api-type: winrt property

---
<!-- Property syntax.
public IObservableVector<ICommandBarElement> SecondaryCommands { get; }
-->

# Microsoft.UI.Xaml.Controls.CommandBarFlyout.SecondaryCommands


## -description

Gets the collection of secondary command elements for the [CommandBarFlyout](commandbarflyout.md).


## -property-value

The collection of secondary command elements for the [CommandBarFlyout](commandbarflyout.md). The default is an empty collection.


## -remarks
The SecondaryCommands collection can directly contain only [AppBarButton](appbarbutton.md), [AppBarToggleButton](appbartogglebutton.md), or [AppBarSeparator](appbarseparator.md) command elements.  Other elements must be wrapped in an [AppBarElementContainer](appbarelementcontainer.md).

The secondary commands are shown in the menu portion of the flyout when the [CommandBarFlyout](commandbarflyout.md) is expanded.


## -see-also

[PrimaryCommands](commandbarflyout_primarycommands.md)


## -examples


## -xaml-syntax

```xaml
<CommandBarFlyout>
    <CommandBarFlyout.SecondaryCommands>
       commandBarElements
    </CommandBarFlyout.SecondaryCommands>
</CommandBarFlyout>
```


## -xaml-values

<dl><dt>commandBarElements</dt><dd>commandBarElementsOne or more object elements for classes that implement ICommandBarElement. These are typically AppBarButton, AppBarToggleButton or AppBarSeparator elements.</dd>
</dl>


