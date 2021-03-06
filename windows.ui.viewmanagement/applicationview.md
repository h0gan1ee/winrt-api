---
-api-id: T:Windows.UI.ViewManagement.ApplicationView
-api-type: winrt class
---

<!-- Class syntax.
public class ApplicationView : Windows.UI.ViewManagement.IApplicationView, Windows.UI.ViewManagement.IApplicationView2, Windows.UI.ViewManagement.IApplicationView3, Windows.UI.ViewManagement.IApplicationView4
-->

# Windows.UI.ViewManagement.ApplicationView

## -description

Represents the active application view and associated states and behaviors.

## -remarks

A window (also called an **app view**) is the displayed portion of a Windows Runtime app. On Windows, a user's screen can have up to 4 windows of variable width displayed simultaneously. They do not overlap, and their top and bottom edges touch the top and bottom edges of the screen. There may be non-window areas between adjacent windows.

The window is not the same thing as the current page of the application. It is better thought of as the container of the pages; you can use the window reference in your program for all the pages of the application.

Each window has a corresponding [CoreWindow](../windows.ui.core/corewindow.md) that represents the UI processing thread (including the core input handlers and event dispatcher) for the window.

You can use the properties (or methods, for JavaScript) of the window in configuring your pages. For example: the [Orientation](applicationview_orientation.md) property tells you whether the window is portrait or landscape; for Windows the [AdjacentToLeftDisplayEdge](applicationview_adjacenttoleftdisplayedge.md) property tells you whether the left edge of the screen is the left border of the window; and the [isFullScreen](applicationview_isfullscreen.md) method tells you whether the window uses the entire screen. For examples of using these methods, see the [Application Views](http://code.msdn.microsoft.com/windowsapps/Application-Views-98825022) sample.

To obtain an object of this type, call [ApplicationView.GetForCurrentView](applicationview_getforcurrentview.md).

> [!NOTE]
> Do not use the value returned in the [ ApplicationView.Value](applicationview_value.md) property when creating a page layout. This method is deprecated and may not be available in future releases.

## -examples

## -see-also

[Disabling screen capture sample (Windows 10)](http://go.microsoft.com/fwlink/p/?LinkId=624047), [User interaction mode sample (Windows 10)](http://go.microsoft.com/fwlink/p/?LinkId=619894), [Multiple views sample (Windows 10)](http://go.microsoft.com/fwlink/p/?LinkId=620574), [Full screen mode sample (Windows 10)](http://go.microsoft.com/fwlink/p/?LinkId=620546), [Window resizing sample (Windows 10)](http://go.microsoft.com/fwlink/p/?LinkId=620026), [Title bar sample (Windows 10)](http://go.microsoft.com/fwlink/p/?LinkId=620613)