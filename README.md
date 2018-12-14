# μDuck

μDuck is stealth HID injector. It's a very small USB device that acts like a scripted keyboard. This can be used for automation and lulz, and has obvious security implications. It's quite similar in functionality to the [Hak5 Rubber Ducky](https://hakshop.com/products/usb-rubber-ducky-deluxe), and even uses the [same syntax](https://github.com/hak5darren/USB-Rubber-Ducky/wiki/Payloads) to define the scripted input.

When μDuck is connected, it will wait 2 seconds in programming mode before switching to a keyboard. This is to allow the payload to be updated with the Python tool provided. It will wait 5 seconds before the first HID injection, then retry the payload automatically at 60 seconds, 5 minutes, and then every 4 hours with +/- 1 hour of random variance. This ensures reliable delivery, but expect that your payload may run more than once.

## Building a μDuck

See the README file in the doc directory.