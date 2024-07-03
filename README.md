# Delta One Internship Projects

## Summary

This repository includes APK files for two projects: DeltaScannerV2 and DeltaMauiScanner. For original source code, visit:
- DeltaScannerV2: [DeltaScannerV2](https://github.com/angryserpicle/TheDeltaScannerV2)
- DeltaMauiScanner: [DeltaMauiScanner](https://github.com/angryserpicle/DeltaMauiScanner)

## Attributes

### DeltaScannerV2
- Includes RFID, Barcode, and Honeywell Swift Decoding Software.
- Requires Android SDK 29 or higher and is optimized for Zebra or Honeywell devices. Refer to the "Steps for Use" section in the [DeltaScannerV2](https://github.com/ElijahH07/TheDeltaScannerV2) for detailed configuration requirements.

### DeltaMauiScanner
- Features a barcode game mode and RFID inventory testing.
- Utilizes the remote Bluetooth RFD40 Zebra Scanner, enabling any Android device to run the app.
- Compatible with any Android device with Bluetooth capabilities. For other operating systems like iOS, refer to the [DeltaMauiScanner](https://github.com/ElijahH07/DeltaMauiScanner) for further details.

---

## Project Report
  The Microsoft Maui Platform is both challenging and an amazing system to work with. It was definetly a challenge to move from the simplicity of Android Studio to the complicated Visual Studio, as well as transitioning from Java to C#. I will break this Report into different sections, analyzing the strengths and weaknesses of the Maui .NET framework.

### XAML/XML Layouts
  XAML layouts in Maui turned out to be straightforward and user-friendly. While remembering slightly different tags can be annoying, the documentation provided is clear and easy to follow. Each button can be assigned an onclick attribute to specify the function to be executed upon clicking. Maui uses sender and event arguments to specify the context and action, which is intuitive and, in my opinion, more efficient compared to setting onClick listeners in Android. Android gracefully provides users with the option to have a live preview whilst editting the XML files compared to .NET MAUI, which forced us to successfully build the solution before making changes to the UI. In terms of the organization and flexibility of using the different layouts, they were both simple and easy to use.

### System Architecture
 Each Maui platform allows for coding the general layout and design of the app while incorporating specific features for different platforms. First, the app initializes an App Shell that loads the main page. Navigation between pages is achieved using the Navigation.PushAsync() function. One interesting aspect is that if the app lags and the user clicks a button multiple times to navigate to another page, Maui may initialize multiple instances of that page. In contrast, Android Studio typically manages a single instance of each page's Intent, creating and deleting instances as needed. For incorporating platform-specific features, Maui offers a straightforward approach by creating partial classes. When compiled for each device, only the code corresponding to the Platform the app is running on is used. This approach enables maintaining a unified app structure while also integrating platform-specific functionalities.

### Devices
  In order to test the two projects, we utilized the Zebra MC33U, Zebra MC930P, Zebra RFD40, and Honeywell CT45P for programming and debugging purposes. Overall, both programs work on all of these devices, using the RFD40 for the RFID Mode for the Zebra and Honeywell devices.

## Conclusion
  Throughout this journey, we have grown significantly as programmers and as a team. Delving into the world of scanners has expanded our understanding and capabilities. We’ve learned the intricacies of C#, explored various software tools, and honed our skills in creating custom solutions for our project.

Our collaboration has been invaluable. Together, we’ve tackled challenges, shared knowledge, and supported each other’s growth. This experience has not only enhanced our technical skills but also strengthened our teamwork and problem-solving abilities.

