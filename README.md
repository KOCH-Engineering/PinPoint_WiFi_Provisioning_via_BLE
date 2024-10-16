
<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<img src="images/13-pin-iso-11446.png" alt="13-pin connector">


<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li><a href="#getting-started">Getting Started</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
    <li><a href="#iso-11446">ISO 11446</a></li>
    <li><a href="#pin-definitions">Pin Definitions</a></li>
    
  </ol>
</details>


<!-- ABOUT THE PROJECT -->
## About The Project

This covers a wireless 13-pin Car Connector Tester using BlueTooth Low Energy Link (BLE)

<h3>In this version the connection is using Wi-Fi which is provisioned using BLE and a mobile App and a QR code</h3>

You insert a plug in the cars connector and this power a wireless transmitter that you can connect to from you mobile phone
The plug powers up the BLE link from the permanent +12V from the plug

You can then see the status on all pins via the user interface on your phone without a cable out of the door.

The Tester will have different modes:
* Mode 1: A graphical representation of the Connector where each pin lights up when 12V og GND is connected
* Mode 2: A Table list structured in groups (ie. Blink Left, Blink Right near to each other
* Mode 3: A latching mode - So the that has been tested stays on
* Mode 4: FUTURE: Connection to CAN bus so that the tester and initiate each test by itself

:smile:

### Built With

This section list major frameworks that were used to build the project
* [Arduiono IDE 2.3.3](https://www.arduino.cc/en/software)

The development board is an ESP32S3 with the module EPS32-S3-WROOM-1 onboard
The chosen board in Arduino IDE is "ESPS3S3 Dev Module"
To be able to have enough room for the code, you have to set Tools|Partition Scheme to "Huge APP (3MB No OTA/1MB SPIFFS)"

When the code has been uploaded to the board the code sends out Serial (115200 baud) data on the COM port on the board


<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

<!-- ROADMAP -->
## Roadmap
See the [open issues](https://github.com/othneildrew/Best-README-Template/issues) for a list of proposed features (and known issues).

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.


<!-- CONTACT -->
## Contact

Henrik Johansen Koch - [@henrikjkoch](https://x.com/henrikjkoch) - henrik@koch-engineering.com

Project Link: [[https://github.com/henrikkoch/13_pin_socket_tester/]](https://github.com/henrikkoch/13_pin_socket_tester/)


<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements
* [Github](https://www.github.com)
* [Arduino](https://www.arduino.cc/)
* [Link to Wifi Provisioning via BLE example](https://randomnerdtutorials.com/esp32-wi-fi-provisioning-ble-arduino/)
* [Link to BLE Code Examples](https://randomnerdtutorials.com/esp32-web-bluetooth/)


## ISO 11446
* [Link to the ISO 11446 standard](https://en.wikipedia.org/wiki/ISO_11446)

ISO 11446:2004 specifies a 13-pole electrical connector between towing and towed vehicles with 12 volt electrical system. It was developed in 1987 by [Erich Jaeger](https://www.erich-jaeger.com/en/products/standards/iso-11446/iso-11446-scope-and-application) to replace older 7-pin plugs.
 

## Pin Definitions

<img src="images/csm_Kontaktbelegung_ISO11446_Rueckseite_2_156baa0ce3.png" width="25%" height="25%"><img src="images/csm_Kontaktbelegung_ISO11446_Front_Stecker_7d4d91d3fa.png" width="25%" height="25%">


<li>Pin 1	 Left indicator [Blink Venstre]</li>
<li>Pin 2	 Rear fog lamp [Tågelys bag]</li>
<li>Pin 3	 Ground [a]<tab>Stel</li>
<li>Pin 4	 Right indicatorBlink Højre</li>
<li>Pin 5	 Right tail lamp [b]Højre baglys</li>
<li>Pin 6	 Brake lamp<tab>Bremselys</tab></li>
<li>Pin 7	 Left tail lamp[b]</li>
<li>Pin 8	 Reverse lamp</li>
<li>Pin 9	 Permanent power</li>
<li>Pin 10	Switched supply (for fridge)</li>
<li>Pin 11	Ground for pin 10 [a]</li>
<li>Pin 12	Trailer Presence Detection[c]</li>
<li>Pin 13	Ground for pin 9 [a]</li>


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/henrikjkoch/
[product-screenshot]: images/screenshot.png
