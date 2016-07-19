# Office 365 Connect Sample for Android Using Microsoft Graph

![Build Status](https://ricalo.visualstudio.com/_apis/public/build/definitions/06256fa7-d8e5-4ca0-8639-7c00eb6f1fe9/7/badge)

[![Office 365 Connect sample](/readme-images/O365-Android-Connect-video_play_icon.png)](https://www.youtube.com/watch?v=3IQIDFrqhY4 "Click to see the sample in action")

Connecting to Office 365 is the first step every Android app must take to start working with Office 365 services and data. This sample shows how to connect and then call one API through the Microsoft Graph (previously called Office 365 unified API).
> Note: Try out the [Get started with Office 365 APIs](http://dev.office.com/getting-started/office365apis?platform=option-android#setup) page which simplifies registration so you can get this sample running faster.

## Device requirements

To run the Connect sample, your device needs to meet the following requirements:

* A screen size of 800 x 480 or larger.
* Android API level 15 or higher.
 
## Prerequisites

To use the Office 365 Connect sample for Android, you need the following:

* [Android Studio](http://developer.android.com/sdk/index.html) version 1.0 or later.
* [Java Development Kit (JDK) 7](http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html).
* An Office 365 account. You can sign up for [an Office 365 Developer subscription](https://profile.microsoft.com/RegSysProfileCenter/wizardnp.aspx?wizid=14b845d0-938c-45af-b061-f798fbb4d170&lcid=1033) that includes the resources that you need to start building Office 365 apps.

     > Note: If you already have a subscription, the previous link sends you to a page with the message *Sorry, you can’t add that to your current account*. In that case use an account from your current Office 365 subscription.
* A Microsoft Azure tenant to register your application. Azure Active Directory provides identity services that applications use for authentication and authorization. A trial subscription can be acquired here: [Microsoft Azure](https://account.windowsazure.com/SignUp).

     > Important: You will also need to ensure your Azure subscription is bound to your Office 365 tenant. To do this see the Active Directory team's blog post, [Creating and Managing Multiple Windows Azure Active Directories](http://blogs.technet.com/b/ad/archive/2013/11/08/creating-and-managing-multiple-windows-azure-active-directories.aspx). The section **Adding a new directory** will explain how to do this. You can also see [Set up your Office 365 development environment](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription) and the section **Associate your Office 365 account with Azure AD to create and manage apps** for more information.
      
* A client id and redirect uri values of an application registered in Azure. This sample application must be granted the **Send mail as a user** permission for **Microsoft Graph**. [Add a native client application in Azure](https://msdn.microsoft.com/office/office365/HowTo/add-common-consent-manually#bk_RegisterNativeApp) and [grant proper permissions](https://github.com/OfficeDev/O365-Android-Microsoft-Graph-Connect/wiki/Grant-permissions-to-the-Connect-application-in-Azure) to it.

## Open the sample using Android Studio

1. Install [Android Studio](http://developer.android.com/sdk/index.html) and add the Android SDK packages according to the [instructions](http://developer.android.com/sdk/installing/adding-packages.html) on developer.android.com.
2. Download or clone this sample.
3. Start Android Studio.
	1. Close any projects that you might have open, and then choose **Open an existing Android Studio project**.
	2. Browse to your local repository and choose the O365-Android-Microsoft-Graph-Connect project. Click **OK**.
	
	> Note: Android Studio might display a dialog box asking if you want to use Gradle wrapper. Click **OK**.
	> 
	> Additionally, Android Studio shows a **Frameworks detected** notification if you don't have the **Android Support Repository** installed. Open the SDK manager and add the Android Support Repository to avoid the Frameworks detected notification.
4. Open the Constants.java file.
	1. Find the CLIENT_ID constant and set its String value equal to the client id you registered in Azure Active Directory.
	2. Find the REDIRECT_URI constant and set its String value equal to the redirect URI you registered in Azure Active Directory.
    ![Office 365 Connect sample](/readme-images/O365-Android-Connect-Constants.png "Client ID and Redirect URI values in Constants file")

    > Note: If you have don't have CLIENT_ID and REDIRECT_URI values, [add a native client application in Azure](https://msdn.microsoft.com/library/azure/dn132599.aspx#BKMK_Adding) and take note of the CLIENT\_ID and REDIRECT_URI.

Once you've built the Connect sample, you can run it on an emulator or device. Pick a device with API level 15 or higher from the **Choose device** dialog.

To learn more about the sample, see [Call Microsoft Graph in an Android app](https://graph.microsoft.io/en-us/docs/platform/android).

<a name="contributing"></a>
## Contributing ##

If you'd like to contribute to this sample, see [CONTRIBUTING.MD](/CONTRIBUTING.md).

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Questions and comments

We'd love to get your feedback about the Office 365 Android Connect project. You can send your questions and suggestions to us in the [Issues](https://github.com/OfficeDev/O365-Android-Microsoft-Graph-Connect/issues) section of this repository.

Questions about Office 365 development in general should be posted to [Stack Overflow](http://stackoverflow.com/questions/tagged/Office365+API). Make sure that your questions or comments are tagged with [Office365] and [API].

## Next steps

This sample just shows the essentials that your apps need to work with Office 365. There is so much more that your apps can do using the Office 365 APIs, like helping your users to manage their work day with calendar, find just the information they need in all the files they store in OneDrive, or find the exact person they need from their list of contacts. We have more to share with you in the [Office 365 APIs Starter Project for Android](https://github.com/officedev/O365-Android-Start/). We think it can help you fuel your ideas. 
  
## Additional resources

* [Office 365 APIs platform overview](https://msdn.microsoft.com/office/office365/howto/platform-development-overview)
* [Getting started with Office 365 APIs](http://dev.office.com/getting-started/office365apis)
* [Office 365 Microsoft Graph overview](http://graph.microsoft.io)
* [Office 365 SDK for Android](https://github.com/OfficeDev/Office-365-SDK-for-Android)
* [Office 365 APIs starter projects and code samples](https://msdn.microsoft.com/office/office365/howto/starter-projects-and-code-samples)
* [Office 365 Android Microsoft Graph Snippets](https://github.com/OfficeDev/O365-Android-Microsoft-Graph-Snippets)
* [Office 365 APIs Starter Project for Android](https://github.com/OfficeDev/O365-Android-Start)
* [Office 365 Profile sample for Android](https://github.com/OfficeDev/O365-Android-Profile)


## Copyright
Copyright (c) 2016 Microsoft. All rights reserved.
