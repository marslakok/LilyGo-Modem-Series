
<div align="center" markdown="1">
  <img src="../../../../../.github/LilyGo_logo.png" alt="LilyGo logo" width="100"/>
</div>

<h1 align = "center">🌟LilyGo SIM7000 Upgrade Guide🌟</h1>

## Resources

- [SIM7000 FlashTools v1.4.3](https://drive.google.com/file/d/1-ADY7_fbXehiQBJZhwp7Kht-ZQpFE1np/view?usp=sharing)
- [SIM7000 Driver](https://drive.google.com/file/d/1f02TTNoyirFPGWbob1khy9dnoBonoVe7/view?usp=sharing)
- [1529B11V01SIM7000G Fixed MQTTS,HTTPS](https://drive.google.com/file/d/12rZ9b7z3ONCPwtevOcz3khYl5vw4zGL3/view?usp=sharing)
- [Tools and files for backing up and restoring QCN](https://drive.google.com/drive/folders/10Fik8zT4UFX1dmCLbZ0GkgIIsxu356QT)

> \[!IMPORTANT]
> Backing up and restoring QCN tools and files only requires downloading and viewing when there are problems with the upgrade. These operations are not required for normal upgrades.
>


### To solder the USB to the upgrade solder joint, you can choose a flying lead or directly solder the USB to the contact

### Power on the SIM7000G board, and at the same time connect the USB interface to the computer port (please note that you need to insert the SIM card during the upgrade process)

![](./images/16.png)
![](./images/17.png)

### Download [SIM7000X Driver](https://drive.google.com/file/d/1f02TTNoyirFPGWbob1khy9dnoBonoVe7/view?usp=sharing), and decompress the corresponding compressed package according to the system you are using

### Open the computer device manager and follow the steps below to add the driver

![](./images/18.png)
![](./images/19.png)
![](./images/20.png)
![](./images/21.png)
![](./images/22.png)
![](./images/23.png)
Follow the above steps to install the driver for the remaining ports that are not installed.
![](./images/24.png)

### Unzip `SIM7000-Update-tools.7z`

### Open `setup.exe` , install update tools , follow the steps below to install

![](./images/1.png)
![](./images/2.png)
![](./images/3.png)
![](./images/4.png)
![](./images/5.png)
![](./images/6.png)
![](./images/7.png)
![](./images/8.png)

### Open the upgrade tool and follow the diagram below

> \[!IMPORTANT]
> If the tool you are using has the QCN backup and restore option, please do not check it.
>

![](./images/9.png)
![](./images/10.png)
![](./images/11.png)
![](./images/12.png)
![](./images/13.png)
![](./images/14.png)
![](./images/15.png)
![](./images/25.png)
![](./images/26.png)

Note that when the following figure is executed, it will prompt that the new port has no driver installed. After adding the driver according to the above steps to install the driver, click Start again to update.

![](./images/27.png)

When prompted `Update Success!`, click Stop to stop the update. At this point, the firmware update has been completed.

![](./images/28.png)

### Open the serial terminal tool, or the built-in serial tool of `Arduino IDE`, select `AT Port` for the port, and enter `AT+CGMR` to view the firmware version

![](./images/29.png)

### Note

If you need to update the 7070G internal firmware, please select the model below to update

![](./images/7070g.png)

Note: the modem must be kept powered on during the procedure; upload an appropriate sketch such as `ATdebug`
