# Egg LDO 250

<table>
  <tr>
    <td><img src="https://github.com/Plaenkler/Egg_LDO_250/assets/60503970/0bc95c62-b583-4c91-be41-ed8abd3cf56e"></td>
    <td><img src="https://github.com/Plaenkler/Egg_LDO_250/assets/60503970/9b1933c9-ae9a-4d60-b8ee-5cebc0db95cc"></td>
  </tr>
</table>

## 📖 What is LDO 250?

The **LDO 250** is the first board in the modular **EGG** design series. The **EGG** series is a conceptual compilation of many different modules.
Modules are created from independent circuit parts which have repeatedly appeared in my PCB designs.
Each of my circuits starts with the voltage source which is why **LDO 250** provides a linear voltage regulator with a low dropout voltage and a maximum current of 250 mA.

## ⚡ Circuit diagram

![Schematics](https://github.com/Plaenkler/Egg_LDO_250/assets/60503970/ec083e19-5229-4551-93cf-a9c46f9f26b0)

## 🔌 Components

### USB-C connector

The 6-pin USB-C connector *USB4135-GF-A* can be sufficient for power supply in scenarios where space is limited and only basic USB functions are required.
This simplified version of the standard USB-C connector provides the essential connections for the power supply and is therefore ideal for small IoT projects.

### Low-dropout regulator

The *MCP1700T-3302E_TT* is a suitable low dropout regulator (LDO) for IoT projects as it provides a stable 3.3V output voltage.
As an LDO, it enables efficient voltage regulation even with small differences between input and output voltage.
It is also characterized by protective functions such as thermal overload protection.

### Resistors

The *RK73B2ATTD512J* (5.1K resistors) are used on a USB-C port to designate the device as a Downstream Facing Device (DFD) or UFP (USB Type-C Female Plug).
This configuration signals to chargers or host devices that a device is connected that requires power.

### Capacitors

With the MCP1700T-3302E/TT, *C0805C106K8PACTU* (10 μF 10V) is used at both the input and output.
A capacitor is used at the input to stabilize the input voltage and filter high-frequency noise.
At the output, the capacitor is used to maintain a stable output voltage and to compensate for rapid load changes.
