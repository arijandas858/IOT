# Raspberry Pi 5 – Temperatūros ir drėgmės matavimas (DHT11)

Šis projektas naudoja **Raspberry Pi 5** ir **DHT11** sensorių aplinkos temperatūrai bei drėgmei matuoti ir atvaizduoti konsolėje.

---

## Funkcionalumas
- Temperatūros matavimas (°C)
- Santykinės drėgmės matavimas (%)

---

## Naudota įranga
- Raspberry Pi 5
- DHT11 temperatūros ir drėgmės sensorius
- Jungiamieji laidai

---

## Naudotos technologijos
- Python 3
- Raspberry Pi OS
- Adafruit DHT biblioteka

---

## Jungimo schema

| DHT11 | Raspberry Pi |
|------|--------------|
| VCC  | 3.3V (Pin 1) |
| DATA | GPIO4 (Pin 7) |
| GND  | GND (Pin 6) |

---

## Diegimas

1. Atnaujink sistemą:
```bash
sudo apt update && sudo apt upgrade
sudo apt install python3-pip
pip3 install adafruit-circuitpython-dht
sudo apt install libgpiod2
Naudojimas

Paleisk programą:

python3 main.py


Pavyzdinė išvestis:

Temperatūra: 22.5°C
Drėgmė: 48%
