



<h1 align="center">ZTE-ROTATE</h1>
<p align="center">
<img src="https://i.ibb.co/rc6cxfM/wheel.png" width="50%">
</p>
This project is a strange way to solve problem with rotating IP addresses on 4g modems.
I tried to use three ways:
<p></p>
<p> </p>

| Way                                      | Problem                                                                                                                          |
|------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
| Use ubuntu usb power control             | Even when device is disconnected it supplied with power                                                                          |
| Use AT commands to reboot device         | In according with MF79U it hasn't any AT commands for rebooting. Another commands not works... I can only know the device number |
| Use fetch with help of browser interface | Every request calculate hash sum with unknown parameters and js compiled so i can't find that data to recalculate                |


I solve to provide restarting with browser automations. My raspberry can run it (rock pi 4a).
I didn't find lightweight browser, so decide to use Firefox with gecko. But i don't want install a python
and want control it in a http-way. This is cause of golang in use.



| script                                                                                      | Behaviour                                                                             | Location                       |
|---------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------|---------------------------------|
| download and install geckodriver from source due to strange rock only that way works for me | Go to github page of geckodriver, takes version and do wget don't checks dependencies | /scripts/download_geckodriver.sh |









