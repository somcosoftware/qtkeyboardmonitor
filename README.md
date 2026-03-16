![Qt Keyboard Monitor](./pictures/QtKeyboardMonitor.png)

# QtKeyboardMonitor
App written with Qt to track keyboard usage on Windows.

It uses windows libraries to detrmine state of keyboard (and also mouse) buttons.
By using those libraries the keyboard state can also be tracked in the background.

---

[![Somco Software](./pictures/Group%201.png)](https://somcosoftware.com)

[![Built with Qt](./pictures/built-with-qt.png)](https://qt.io)

---

User don't have to be focused on window for the tracking to take place - it can eaven be minimalized.
The keys state are checked every time the timer is triggered. Timer is triggered every 100ms.
User activity is measured with three variablem APS, APM and avarageAps.

- APS variable stands for Actions Per Second. It's number of buttons pressed by user every second. APS is updated every second.
- APM variable stands for Actions Per Minute. It's sum of the number of keys presses on the keyboard, per minute. As expected variable is updated every minute.
- AvarageAPS is just avarage number of actions per second. It is updated every minute. Avarage is counted simply by deviding current APM value by 60.

# How to use
To see the example simply clone this repository and simply run the project - no additional configuration is needed.

If you want to reuse this code in a QML app, simply create proper C++ class with code from KeyboardMonitor.cpp and KeyboardMonitor.h and then, add context to QML engine with this line:

`engine.rootContext()->setContextProperty("keyboardMonitor", keyboardMonitor);`

Now you can use keyboard monitor from the QML level. For examples how to use it, see main.qml file.

# Licence
This project is licensed under the MIT License - see the LICENSE.txt file for details.
 
 DISCLAIMER: Somco Software does not bear responsibility for inappropriate or malicious use of code in this project

## About Somco Software (previously Scythe Studio)
[Somco Software](https://somcosoftware.com/en/) (previously Scythe Studio) is an embedded and cross-platform software development company with a strong focus on Qt and C++, delivering reliable, high-quality solutions for regulated industries, with particular expertise in medical devices. We are an ISO 9001 and ISO 13485 certified software house, specializing in GUI development, Linux-based systems, and advanced connectivity solutions. Somco Software is an official Qt Service Partner and a trusted partner of leading hardware manufacturers.

<table style="margin: 0 auto; border:0;">
    <tr style="border:0">
        <td style="border:0">
            <a href="https://somcosoftware.com">
            <img width="340" height="150" src="./pictures/Qt-service-partner-badge.png">
            </a>
        </td>
        <td style="border:0">
            <a href="https://clutch.co/profile/scythe-studio">
                <img height="150" width="150"
                    src="https://github.com/user-attachments/assets/023e102e-84c1-4e7e-b9de-cae476e681e7">
            </a>
        </td>
        <td style="border:0">
            <a href="https://scythe-studio.com/en/iso">
                <img src="./pictures/iso 13485.png">
            </a>
        </td>
        <td style="border:0">
            <a href="https://scythe-studio.com/en/iso">
                <img src="./pictures/iso 9001.png">
            </a>
        </td>
    </tr>
</table>

We support projects from design to delivery, offering UX/UI design, custom Yocto Linux images, and development in Qt as well as LVGL and TouchGFX. We also help with software modernization, training, and technical consulting. With a practical, developer-focused approach, we build efficient, reliable solutions that fit real project needs.

# Professional Support
Need help with anything? We’ve got you covered. Our professional support services are here to assist you with. For more details about support options and pricing, just drop us a line at https://somcosoftware.com/en/contact.

# Follow us
Check out those links if you want to see Somco Software in action and follow the newest trends saying about Qt Qml development.

* 🌐 [Somco Software Website](https://somcosoftware.com/en/)
* ✍️ [Somco Software Blog Website](https://somcosoftware.com/en/blog)
* 👔 [Somco Software LinkedIn Profile](https://www.linkedin.com/company/somcosoftware)
* 🎥 [Somco Software Youtube Channel](https://www.youtube.com/channel/UCf4OHosddUYcfmLuGU9e-SQ/featured)

