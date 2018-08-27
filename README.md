# HololensSampleCodes
This README shows how to make [Hololens sample codes by Microsoft](https://github.com/Microsoft/HoloLensForCV) run. 

## Environment and Software Requirement
- Visual Studio 2017 Update 3
- Windows 10 April 2018 Update

## Build and Deploy Settings

0. Before we start, connect the Hololens to your computer over Wi-Fi or USB

1. Enable **Developer Mode** on your computer (go to **Settings > Update & Security > For developers**)
    1. Set **Use developer features** to On
    2. Set **Enable Device Portal** to On
    
2. Setting up HoloLens to use **Device Portal**
    1. On Hololens, go to **Settings > Update > For Developers**
    2. Enable **Developer Mode**
    3. Enable **Device Portal**
    4. During your first time App deployment to the Hololens via USB or Wi-Fi, Visual Studio will ask for the PIN code. Now in the **For Developers** page on Hololens, click **Pair** to generate a pairing PIN and enter it in Visual Studio.
    
3. Connect to **Device Portal** on computer
    > The first time you connect to the Device Portal on your computer, you will need to create a username and password.
    1. In a web browser on your PC, enter the IP address ([over USB](https://docs.microsoft.com/en-us/windows/mixed-reality/using-the-windows-device-portal#connecting-over-wi-fi), [over Wi-Fi](https://docs.microsoft.com/en-us/windows/mixed-reality/using-the-windows-device-portal#connecting-over-usb)) of the HoloLens. The Set up access page opens. (If not, try to click "yes" in the pop-up login windows for several times)
    2. Get the generated PIN in Hololens
    3. Enter the PIN
    4. Enter the user name you will use to connect to the Device Portal. It doesn't need to be a Microsoft Account (MSA) name or a domain name
    5. Enter a password and confirm it. The password must be at least seven characters in length. It doesn't need to be an MSA or domain password
    6. Click Pair to connect to Windows Device Portal on the computer
    
4. Enable **Allow access to sensor streams** in Device Portal on the computer
    1. Open a web brower and go to the Device Portal
    2. Go to **System > Research Mode**
    3. Set **Allow access to sensor streams** to On 
    4. Reboot Hololens
    
5. Now the sample apps should work fine in the Hololens after you build and deploy the apps with Visual Studio. 
