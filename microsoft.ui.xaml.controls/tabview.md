---
-api-id: T:Microsoft.UI.Xaml.Controls.TabView
-api-type: winrt class
---

## -description

The TabView control is a way to display a set of tabs and their respective content. Tab controls are useful for displaying several pages (or documents) of content while giving a user the capability to rearrange, open, or close new tabs. 

**Is this the right control?**

Use a TabView to help the user manage multiple app pages or documents within the same window. 

Do not use a TabView to display a static set of tabs that the user cannot rearrange, open, or close. Use a Pivot or top NavigationView instead. 

## -remarks

## -see-also

## -examples

> [!TIP]
> For more info, design guidance, and code examples, see [Tab view](/windows/uwp/design/controls-and-patterns/tab-view).
>
> If you have the **XAML Controls Gallery** app installed, click here to [open the app and see the TabView in action](xamlcontrolsgallery:/item/TabView).
> + [Get the XAML Controls Gallery app (Microsoft Store)](https://www.microsoft.com/store/productId/9MSVH128X2ZT)
> + [Get the source code (GitHub)](https://github.com/Microsoft/Xaml-Controls-Gallery)

### Basic TabView Sample, similar to a Web Browser

``` xml
<TabView AddTabButtonClick="Tabs_AddTabButtonClick"
         TabCloseRequested="Tabs_TabCloseRequested" />
```

``` csharp
// Add a new Tab to the TabView
private void Tabs_AddTabButtonClick(TabView sender, TabViewAddTabButtonClickEventArgs e)
{
    var newTab = new TabViewItem();
    newTab.IconSource = new SymbolIconSource() { Symbol = Symbol.Document };
    newTab.Header = "New Document";

    // The Content of a TabViewItem is often a frame which hosts a page.
    Frame frame = new Frame();
    newTab.Content = frame;
    frame.Navigate(typeof(BaconIpsumPage));

    sender.TabItems.Add(newTab);
}

// Remove the requested tab from the TabView
private void Tabs_TabCloseRequested(TabView sender, TabViewTabCloseRequestedEventArgs args)
{
    sender.TabItems.Remove(args.Tab);
}
```
