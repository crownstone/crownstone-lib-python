# crownstone-lib-python
Python library to interact with the Crownstone system

We have split our python library into smaller segments for maintainability as well as API clarity.

So which one do you need?

## Cloud
Here you can easily get your Spheres, rooms and Crownstones from our cloud server. You can also switch a Crownstone via the cloud. This will send push notifications to the phones in the sphere, which will then switch the Crownstones. If you have a hub device, these can also switch your Crownstones for you if you switch via de cloud lib.

More info here: [crownstone-lib-python-cloud](https://github.com/crownstone/crownstone-lib-python-cloud)

## SSE
If there are changes in the cloud, like users going from room to room, Crownstones being added, Crownstones being switched via the cloud etc, our Server-Sent-Event server can send these events to you in real-time! The SSE library facilitates this for you.

More info here: [crownstone-lib-python-sse](https://github.com/crownstone/crownstone-lib-python-sse)

## UART
If you have a Crownstone USB dongle, you can use the UART library to interact with it. Using the UART library and the USB, you can listen to the mesh network, for power usages, switch states of the Crownstones etc. You can also configure the Crownstones via the mesh, and switch Crownstones directly. These USB devices are commonly used for hubs.

More info here: [crownstone-lib-python-uart](https://github.com/crownstone/crownstone-lib-python-uart)

## BLE
This library only works in Linux due to the BlueZ dependency. Using the BLE lib, you can connect to Crownstones, scan for their state updates, powerusage etc. We recommend using a dedicated bluetooth dongle, since they are much more stable than common, onboard bluetooth. For better performance and reliability, we recommend the Crownstone USB.

More info here: [crownstone-lib-python-ble](https://github.com/crownstone/crownstone-lib-python-ble)

## Core
You do not need this. This is a library with shared definitions for the other libraries.

More info here:[crownstone-lib-python-core](https://github.com/crownstone/crownstone-lib-python-core)
