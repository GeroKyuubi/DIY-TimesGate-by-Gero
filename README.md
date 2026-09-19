
[![Store](https://img.shields.io/badge/Tindie-Store-green.svg)](https://www.tindie.com/stores/gero87/)

# DIY-TimesGate-by-Gero
Bring your desk to life with TimesGate, a compact, fully customizable 4-screen desktop dashboard powered by the ESP32-S3. Whether you want to monitor crypto prices, track forex rates, check live weather, view custom retro pixel art, or keep an eye on world clocks and countdowns, TimesGate puts real-time information right at your fingertips.

A compact, customizable information dashboard powered by ESP32-S3 and four ST7789 color displays.

TimesGate is a DIY smart desktop dashboard designed around an ESP32-S3 and four independent 1.69" 240×280 ST7789 TFT displays.

# Hardware Features & Pinout

Microcontroller: ESP32-S3 DevKit

Displays: 4x ST7789 Color LCD Screens (240x280) connected via an optimized SPI bus.

Physical Buttons:

- BOOT Button (GPIO 0): Used to enter Configuration / Captive Portal mode.
- RESET Button (EN to GND): Performs a physical hardware restart of the board.
- Widget Cycle Button (GPIO 15): Instantly cycles through available widgets on Display 1 (Screen #0) without rebooting.

# First-Time Setup & Wi-Fi Configuration
When you power on TimesGate for the first time—or if no Wi-Fi credentials are saved—it automatically boots into Captive Portal / AP Mode.
1.	Power up the device using a USB-C cable.
2.	Open the Wi-Fi settings on your phone, tablet, or PC and connect to the network named:
👉 TimesGate-DIY
3.	Once connected, a configuration page should open automatically. If it doesn't, open a web browser and go to:
👉 [http://192.168.4.1](http://192.168.4.1)
4.	Fill in your details on the setup page:
- Wi-Fi SSID & Password: Your home/office network credentials.
- Weather Setup: Type your city name (e.g., London, New York, Rome).
- Custom Note: Write a personal text message or memo.
- Countdown Setup: Set an event title and target date/time.
- Custom Pixel Art Editor: Use the interactive 16x16 grid to draw your own retro icon.
- Display Configuration: Assign your preferred widget to each of the 4 screens.
5.	Click SAVE & CONNECT. The device will save your preferences, restart, and connect to your Wi-Fi network.

# Operating the Device
- Normal Operation: Once connected to Wi-Fi, TimesGate synchronizes time via NTP and begins fetching live data for your active widgets.
- Changing Display 1 Widget on the Fly: Press the physical button connected to GPIO 16 to cycle forward through all available widget types on the first screen dynamically.
- Reconfiguring / Changing Wi-Fi: If you need to change your settings or Wi-Fi network later, press and hold the BOOT button (GPIO 0) while the device is running to re-enter the Captive Portal mode.

# Available Widgets
- World Clock: Displays 4 major timezones side-by-side (UTC, CET, EST, CST).
- Demo Counter: A simple incrementing loop counter.
- Matrix Digital Rain: Cyberpunk-style falling green and white characters.
- Open-Meteo Weather: Live vector weather icons, temperature, and relative humidity.
- Forex Rates: Real-time exchange pairs (EUR/USD, EUR/GBP, EUR/CNY, USD/CNY).
- Crypto Tracker: Live prices for Bitcoin (BTC/USD) and Ethereum (ETH/USD).
- Pixel Art Heart & Anime: Retro pre-loaded pixel graphics.
- Notes Widget: Displays multi-line custom notes entered via the WebUI.
- Countdown Widget: Live ticking countdown timer for your special events.
- Custom Pixel Art: Displays your custom drawings made via the WebUI 16x16 editor.
- PhotoFrame: Use a microSD card to display JPEG/JPG photographs on the TFT display, including slideshow implementation with automatic image changes every 60 seconds.

#Still Work In Progress... stay tuned!!!


