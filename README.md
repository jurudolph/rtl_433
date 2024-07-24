# ioBroker - Integration von INKBIRD Sensoren mit 433 MHz RF (Poolsensor IBS-P01R und Temperatur/Feuchtesensor ITH-20R)

Es gibt bereits eine Integration für die beiden o.g. INKBIRD Sensoren über die INKBIRD Gateways IBS-M1 und IBS-M2 unter Verwendung des Tuya-Adapter im ioBroker. Diese Integration erlaubt z.B. auch die Einbindung von Bluetooth – Sensoren wie IBS-P01B. Die gleichzeitige Verbindung der Gateways mit der INKBIRD – Cloud und Nutzung der entsprechenden Apps ist nicht möglich. Das Verfahren ist hier beschrieben https://github.com/jurudolph/Inkbird

Für die o.g. INKBIRD Sensoren mit 433 MHz RF gibt es eine Möglichkeit das RF Signal direkt zu verarbeiten und in ioBroker zu integrieren, ohne INKBIRD Gateway. Nebenbei können die Daten von ca. 250 anderen 433 MHz RF Devices (Temperatur/Feuchtesensoren, Funkfernbedienungen, Reifendrucksensoren, Wetterstationen) empfangen werden.

Benötigt werden:
- ein RTL-SDR (RTL2832U USB Dongle) für ca. 20 € https://www.rtl-sdr.com/
- die generische Datenempfangssoftware rtl_433 (Docker, Linux, Windows, MacOS) https://github.com/merbanan/rtl_433
- ggf. einen kleinen Server auf dem rtl_433 läuft, z.B. ein Raspberry Pi
- der ioBroker MQTT Broker/Server Adapter https://github.com/ioBroker/ioBroker.mqtt

Die Integration mit OpenHAB und Home Assistant über MQTT ist hier beschrieben. Sie ist für ioBroker analog.
https://triq.org/rtl_433/INTEGRATION.html
https://github.com/merbanan/rtl_433/wiki/How-to-integrate-rtl_433-sensors-into-openHAB-via-MQTT

Hilfreich ist auch dieses Video (für openHAB) https://www.youtube.com/watch?v=WwAuQE2Z7h0

Details siehe Anleitung.pdf https://github.com/jurudolph/rtl_433/blob/main/Anleitung.pdf

![image](https://github.com/user-attachments/assets/2c2fe64e-ea08-4089-8537-427c9329ac32)
