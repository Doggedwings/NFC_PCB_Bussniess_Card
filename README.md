# NFC Business Card PCB

A custom PCB business card with an embedded NFC chip, LED, capacitor, and resistor. Hold it near any NFC-enabled phone, and the LED lights up while instantly opening a URL of your choice, no battery required. The card harvests all the power it needs directly from the phone's RF field.
I built this to learn PCB design from scratch and to have something physical I could actually hand to people. It turned into more than that.
After finishing the card I volunteered to bring the project to my high school's STEM Club, running a workshop where over 100 students learned the basics of electronics and PCB design by building their own version. Every student designed a unique card with their own artwork and personality. Through Hack Club's OnBoard grant program every board was manufactured and shipped for free. Handing students their first self-designed PCB and watching them show it off to friends and family made the whole thing worth it.

## How It Works

The NT3H2111 NFC chip harvests energy from the RF field emitted by the reading device. 
This harvested energy powers both the NFC communication and a status LED 
that lights up on tap. The antenna is a tuned spiral coil 
etched directly into the PCB copper layer.

## Specs

- **NFC chip:** NT3H2111W0FHK (NXP) — I2C + energy harvesting
- **Frequency:** 13.56 MHz (ISO 14443A / NFC Forum Type 2)  
- **Antenna:** Custom spiral coil, tuned for 13.56MHz resonance
- **LED:** Lights up on NFC field detection — no battery needed
- **PCB:** 2-layer, 85.5 × 54mm (credit card size), black soldermask
- **Manufactured:** JLCPCB with SMT assembly

## Schematic

<img width="1149" height="809" alt="schematic" src="https://github.com/user-attachments/assets/f03384c3-dba6-4f41-b83a-b7d2bf87c74c" />


## Physical Card

![Bussniess Card Front](https://github.com/user-attachments/assets/8685151f-9900-4d1d-b183-21685ee58bbe)

![Bussniess Card Back](https://github.com/user-attachments/assets/88199816-abcc-43fe-b56c-8997cae0d191)


## What I Learned

- PCB antenna design — tuning a spiral coil for 13.56MHz 
  resonance using capacitor matching
- EasyEDA schematic and layout workflow
- JLCPCB SMT assembly ordering process
- NFC NDEF data format and programming with NFC Tools app
- Energy harvesting circuit design (no battery required)


