<properties
    pageTitle="Release notes for PowerApps | Microsoft PowerApps"
    description="Release notes"
    services=""
    suite="powerapps"
    documentationCenter="na"
    authors="gregli-msft"
    manager="erikre"
    editor=""
    tags=""/>
<tags
    ms.service="powerapps"
    ms.devlang="na"
    ms.topic="article"
    ms.tgt_pltfrm="na"
    ms.workload="na"
    ms.date="04/27/2016"
    ms.author="gregli"/>

# Release notes for PowerApps release 2.0.430 #

For information about known limitations in this release, see [Common issues and resolutions](common-issues-and-resolutions.md).

1. **Update required for PowerApps Studio and PowerApps Mobile**.

	Due to an internal change, you must install this update to continue to create and edit apps in PowerApps Studio and run apps in PowerApps Mobile.

	For Windows 8 and Windows 8.1:

	1.	Open the app for the Windows Store.
	1.	Open the settings for that app.<br>For example, press the Windows key and the “c” key simultaneously, and then select **Settings**.
	1.	Select  **App updates**, and then select **Check for updates**.
	1.	In the screen that appears, select **Install** for PowerApps.

1. **Enhanced delegation for large data sets.**

	- **SortByColumns** now supports delegation.
	- **Sort**, **SortByColumns**, and **Filter** can now be composed together.
	- More support for delegation is on the way.

1. **Updates property added to the Edit form control.**

	The **[Edit form](controls/control-form-detail.md)** control now has an **[Updates](controls/control-form-detail.md)** property to access all the **[Update](controls/control-card.md)** properties of the cards within the form.

	You can use this property to pass form data to a REST API.

1. **Bug fixes for Video control.**

	Now works with YouTube.

1. **Single sign-on support for Microsoft services.**

	Single sign-on feature will automatically sign PowerApps users into their first party services that use Azure Active Directory authentication, such as SharePoint, Office 365, and Dynamics CRM.

1. **Added Edit lookup card.**

	As soon as you install this PowerApps update, **[Display form](controls/control-form-detail.md)** and **[Edit form](controls/control-form-detail.md)** controls will show lookup fields to other tables, but this data will be read-only. As soon as other changes occur in the SharePoint connector, you’ll be able to update these fields for data in SharePoint lists. (You won’t need to update PowerApps again to take advantage of this capability).

1. **Minimum/maximum values for numeric cards.**

	Numeric cards, such as those for ratings and percentages, reflect minimum and maximum values that you set (or that are set in the metadata for the data source).

1. **Default value for the DatePicker control.**

	You can configure a DatePicker control with a blank value as its default.

1. **Improvements to Display Form and Edit Form controls.**

	Form controls now show both a display name and the name of the field if they differ, and you can change the display name of a lookup control.

1. **On powerapps.com, show only those apps you own or were shared with you.**

1. **Bug fixes and performance improvements throughout the product.**

## Release Notes for 2.0.410 ##

### PowerApps.com ###
1. 	**Use apps directly on the web!**

	You can find and use PowerApps on any device that has a web browser.

2.  **A new home screen at PowerApps.com.**

	Features include:
	- Quick access to your apps
	- Sample apps that you can check out to get started
	- Documentation to learn more

3.	**A fresh new look for finding and managing your apps, connections, and notifications.**

4.	**Improvements to the sharing experience.**

	Users can now reshare apps and share apps with their organization.

### PowerApps Mobile ###
1. 	**PowerApps is now available for Android!**

	Look for PowerApps in the [Android store](http://aka.ms/powerappsandroid).

2. 	**PowerApps has a new look for finding and opening apps on devices that run iOS.**

	Update your app or install anew from the [Apple store](http://aka.ms/powerappsios).

3. **Simplified sign-in and first-run experiences.**

4. **Usability improvements.**

	We've added hamburger navigation and an app context menu.

### PowerApps Studio ###

1. **Streamlined page for starting to create an app.**

	- More useful options for quickly getting to what you need.
	- An improved flow, including better breadcrumbs and navigation, when you create an app from data.
	- Now you can see your most recently used SharePoint sites when you create an app from SharePoint Online, for those users who don’t memorize their SharePoint URLs.

3. **New guided product tour.**

	A quick tour of the most important parts of the authoring experience to help new users get acquainted.

1. **Contextual help links.**

	We've made it much easier for you to find help in the product and connect with others through our community.

3. **New [Edit form](controls/control-form-detail.md) and [Display form](controls/control-form-detail.md) controls. As a result, better apps generated from data.**

	Creating an app over data just got a whole lot easier.  With these controls and their associated cards and functions, you can create a basic app to view and edit data without needing to manually call **[Patch](functions/function-patch.md)**, **[Validate](functions/function-validate.md)**, and other low-level functions.

	These controls also offer a new configuration pane, where you can turn on and off fields and change the card for each field.

	Check out [Understand data forms](working-with-forms.md) for more details.

1. **Data-source delegation of [Filter](functions/function-filter-lookup.md) and [Sort](functions/function-sort.md) improves performance and supports large numbers of records.**

	Until now, all Filter and Sort operations were handled on the device, which required the time-consuming and bandwidth-choking fetch of all the data.  With this release, in certain situations, these operations can be delegated to the data source, which makes your apps more responsive and able to handle a large number of records.  You can read more about it on the [Filter](functions/function-filter-lookup.md) and [Sort](functions/function-sort.md) pages.

	Delegation is limited to certain situations. Apps created from data don't qualify.  See [Known limitations](#known-limitations) later in this article for more details.  We will expand the scenarios in which delegation can be used.

	To take advantage of this new capability, the **[Gallery](controls/control-gallery.md)** control now supports paging.  As the user reaches the end of a list of data, the control fetches more from the data source, seamlessly.

1. **Search and scroll in the [PDF viewer](controls/control-pdf-viewer.md) control.**

	The PDF viewer control now supports full-text search across the document, and we've added smooth scrolling between pages. No longer do you need to move page by page.

1. **More connectors.**

	We continue to add connectors. [Check out the list](connections-list.md) for the latest.

1. **Metadata refresh.**

	Update your metadata with a single click or tap (instead of deleting a connection and adding it again).

1. **A list of your most recently used SharePoint sites.**

	Building a bunch of apps for the same SharePoint site? To make that easier, we track SharePoint sites that you've recently used so that you can easily select them again.   

1. **Performance and data-handling improvements, along with many other usability and bug fixes throughout!**

### Connections ###

This release supports these connections, among [many others](connections-list.md):

- SharePoint
- Office 365
- Dynamics CRM
- SQL
- OneDrive for Business
- Dropbox
- Google Drive
- Slack
- Twilio
- Yammer
- Twitter