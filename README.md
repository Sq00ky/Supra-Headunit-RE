### Overview
This repository contains resources related to reverse engineering the Toyota Supra Headunit firmware.
### Remounting the Filesystem as RW
mount -o remount rw /net/hu-omap/fs/sdaX
credit to @a90.faraz
### SSH Connection
Pre-Req: Ethernet -> ODB2 cable (Also known as eNet).
1. Message the guys @ FlashXCode on Whatsapp, be sure to ask them to enable SSH, include your VIN & iStep version number (can be found under Navigation > Settings > Position and software version > software version) - https://www.flashxcode.com/product/feature-installer-code/
2. Paypal them 25 Euros as Friends and Family
3. Download FeatureInstaller
4. Run FeatureInstaller, wait for it to scan then select "Identify" when you've found the car
5. Input the code provided by FlashXCode
6. Wait for it to finish

Afterwards, you can ssh into:
ssh root@169.254.199.99
ts&SK412

### Ownership
All rights belong to Toyota (Toyota Motor Corporation) , BMW (Bayerische Motoren Werke AG), and Harman Kardon (Harman International)
