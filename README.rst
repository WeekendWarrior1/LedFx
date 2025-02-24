=====================================================
   Welcome to LedFx ✨ *- Making music come alive!*
=====================================================
|Build Status| |License| |Build Status Docs| |Discord|
|Contributor Covenant|

.. image:: https://github.com/LedFx/LedFx/blob/b8e68beaa215d4308c74d0c7d657556ac894b707/icons/banner.png

LedFx website: https://ledfx.app/
----------------

What is LedFx?
----------------

**Music to Light!**

LedFx instantaneously transforms audio input into a realtime light show.
No need to spend hours on syncing your LEDs to music - LedFx will do this all for you!

LedFx is a real-time music visualization program that streams audio reactive effects to networked LED strips.
LedFx can control multiple devices and works great with cheap ESP8266/ESP32 nodes, allowing for cost effective synchronized effects across your entire house!

Demos
-------

We are actively adding and perfecting the effects. Here are some of our favourites!

https://user-images.githubusercontent.com/32398028/144685437-4d9224ef-3e5f-4bf4-a754-7aac6dbf1d25.mp4

**⚠ PHOTOSENSITIVE EPILEPSY WARNING ⚠** - The following videos contain rhythmic flashing lights

https://user-images.githubusercontent.com/32398028/144686069-0f818d56-df66-4846-a849-c2f046e83fcf.mp4

https://user-images.githubusercontent.com/32398028/144686116-45b4b4f9-6f4d-4dd8-9caf-26e58fc2357a.mov

https://user-images.githubusercontent.com/32398028/144686803-110c7124-782c-4f39-af90-68e1133309fa.mp4

📑 Quick start guide and documentation📖
------------------------------------------
Windows users can use the installer from the LedFx website: https://ledfx.app/download/

Mac and Linux are also supported, though currently do not have installers.
For detailed installation instructions, see the `installation documentation`_.

😍 Show me how to make one!
-----------------------------

The below image describes a basic setup - LedFx running on PC, communicating with a WLED Device controlling an LED strip.

.. image:: https://i.imgur.com/vzyHNwG.png

.. list-table::
   :widths: 75 75
   :header-rows: 1

   * - Component
     - Example
   * - Computer running LedFx
     - Windows 10, `LedFx.exe`_
   * - Networked device controlling LED Strip
     - ESP8266 NODEMCU v3 running `WLED`_
   * - Addressable LED strip
     - DC5V WS2812B 5 meters 60LED/m IP67
   * - Power supply for LED Strip and ESP
     - 5V 10 amps LED Power Supply
   * - Something to connect the wires together!
     - Soldering iron/solder

#. **Build your networked LED Strip.**
      - For most, this is the difficult step. Don't worry! There's guides here and online, and plenty of people able to help on WLED and LedFx Discord.
      - Follow the WLED guide to connect the LED strip and ESP together: https://github.com/Aircoookie/WLED/wiki.
      - Flash WLED to the ESP device: https://github.com/Aircoookie/WLED/wiki/Install-WLED-binary
      - Ensure all WLED devices are powered on, and connected to your Wi-Fi.
      - Test you can access the WLED web interface from your PC. If so, then you're good to go!

#. **Install LedFx.**
      - After you have WLED installed on your ESP device, download: `LedFx.exe`_ and install LedFx.
      - For Mac and Linux, see the `installation documentation`_ or `LedFx Guide`_.

#. **Direct computer audio output to LedFx.**
      - Follow guide, `How to: Enable Stereo Mix in Windows 10`_.
      - Alternatively use `Voicemeeter`_. `Voicemeeter tutorial`_.
      - More information for `Linux and macOS users here <https://ledfx.readthedocs.io/en/master/directing_audio.html>`_.
      - Play some music in the background.

#. **Start LedFx.**
      - Your WLED devices should appear in LedFx, automagically configured and ready to go! 🎆🔥
      - If not, on the left hand side, click on Device Management -> ``Find WLED devices`` button, or ``Add Device`` to add them manually.
      - If they're still not showing up, make sure they're powered on and properly connected to your WiFi.

#. **Start using effects!**
      - Click on the device, select an effect eg ``scroll(Reactive)``, and press ``Set effect`` button.
      - Your lights should now be reacting realtime to your music! Enjoy the show 🌈


🧑‍💻 Join the LedFx Community
------------------------------

Join the Discord server to discuss everything about LedFx!  |Discord|

To join, click on the Discord button below:

.. image:: https://discordapp.com/api/guilds/469985374052286474/widget.png?style=banner2
   :width: 30%
   :target: https://discord.com/invite/xyyHEquZKQ

Contributing
--------------
Pull requests are welcome. Once tested, contact LedFx developer community on Discord to discuss the next step.
We expect and require all contributors to read, understand and follow our code of conduct.

Credits: `Contributors-&-About`_

License
---------
`MIT`_


.. _`MIT`: https://choosealicense.com/licenses/mit/
.. _`LedFx.exe`: https://ledfx.app/download/
.. _`LedFx Guide`: https://ledfx.readthedocs.io/en/master/index.html
.. _`WLED`: https://github.com/Aircoookie/WLED/wiki
.. _`installation documentation`: https://ledfx.readthedocs.io/en/master/installing.html
.. _`Contributors-&-About`: https://ledfx.app/about/
.. _`How to: Enable Stereo Mix in Windows 10`: https://thegeekpage.com/stereo-mix/
.. _`Voicemeeter`: https://vb-audio.com/Voicemeeter/index.htm
.. _`Voicemeeter tutorial`: https://youtu.be/ZXKDzYXS60o?start=27&end=163

.. |Build Status| image:: https://github.com/LedFx/LedFx/actions/workflows/ci-build.yml/badge.svg
   :target: https://github.com/LedFx/LedFx/actions/workflows/ci-build.yml
   :alt: Build Status
.. |Build Status Docs| image:: https://readthedocs.org/projects/ledfx/badge/?version=master
   :target: https://ledfx.readthedocs.io/
   :alt: Documentation Status
.. |License| image:: https://img.shields.io/badge/license-MIT-blue.svg
   :alt: License
.. |Discord| image:: https://img.shields.io/badge/chat-on%20discord-7289da.svg
   :target: https://discord.gg/xyyHEquZKQ
   :alt: Discord
.. |Contributor Covenant| image:: https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg
   :target: CODE_OF_CONDUCT.md
