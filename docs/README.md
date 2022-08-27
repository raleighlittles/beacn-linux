# dmesg output

```
[Fri Aug 26 12:28:23 2022] usb 1-4.4.2: new high-speed USB device number 18 using xhci_hcd
[Fri Aug 26 12:28:23 2022] usb 1-4.4.2: New USB device found, idVendor=33ae, idProduct=0004, bcdDevice= 1.01
[Fri Aug 26 12:28:23 2022] usb 1-4.4.2: New USB device strings: Mfr=1, Product=2, SerialNumber=3
[Fri Aug 26 12:28:23 2022] usb 1-4.4.2: Product: BEACN Mix
[Fri Aug 26 12:28:23 2022] usb 1-4.4.2: Manufacturer: BEACN
[Fri Aug 26 12:28:23 2022] usb 1-4.4.2: SerialNumber: 0041220400408
[Fri Aug 26 12:28:23 2022] hid-generic 0003:33AE:0004.0009: hiddev1,hidraw7: USB HID v1.00 Device [BEACN BEACN Mix] on usb-0000:00:14.0-4.4.2/input0
```

# lsusb output

```
Bus 001 Device 018: ID 33ae:0004 BEACN BEACN Mix
Couldn't open device, some information will be missing
Device Descriptor:
  bLength                18
  bDescriptorType         1
  bcdUSB               2.00
  bDeviceClass          239 Miscellaneous Device
  bDeviceSubClass         2 
  bDeviceProtocol         1 Interface Association
  bMaxPacketSize0        64
  idVendor           0x33ae 
  idProduct          0x0004 
  bcdDevice            1.01
  iManufacturer           1 BEACN
  iProduct                2 BEACN Mix
  iSerial                 3 0041220400408
  bNumConfigurations      1
  Configuration Descriptor:
    bLength                 9
    bDescriptorType         2
    wTotalLength       0x0029
    bNumInterfaces          1
    bConfigurationValue     1
    iConfiguration          0 
    bmAttributes         0xc0
      Self Powered
    MaxPower                0mA
    Interface Descriptor:
      bLength                 9
      bDescriptorType         4
      bInterfaceNumber        0
      bAlternateSetting       0
      bNumEndpoints           2
      bInterfaceClass         3 Human Interface Device
      bInterfaceSubClass      0 
      bInterfaceProtocol      0 
      iInterface              0 
        HID Device Descriptor:
          bLength                 9
          bDescriptorType        33
          bcdHID               1.00
          bCountryCode            0 Not supported
          bNumDescriptors         1
          bDescriptorType        34 Report
          wDescriptorLength      32
         Report Descriptors: 
           ** UNAVAILABLE **
      Endpoint Descriptor:
        bLength                 7
        bDescriptorType         5
        bEndpointAddress     0x03  EP 3 OUT
        bmAttributes            3
          Transfer Type            Interrupt
          Synch Type               None
          Usage Type               Data
        wMaxPacketSize     0x0400  1x 1024 bytes
        bInterval               1
      Endpoint Descriptor:
        bLength                 7
        bDescriptorType         5
        bEndpointAddress     0x83  EP 3 IN
        bmAttributes            3
          Transfer Type            Interrupt
          Synch Type               None
          Usage Type               Data
        wMaxPacketSize     0x0040  1x 64 bytes
        bInterval               1
```
