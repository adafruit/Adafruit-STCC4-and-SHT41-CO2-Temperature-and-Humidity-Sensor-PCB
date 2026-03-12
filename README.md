## Adafruit STCC4 and SHT41 - CO2, Temperature & Humidity Sensor - STEMMA QT / Qwiic PCB

<a href="http://www.adafruit.com/products/6478"><img src="assets/6478.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit STCC4 and SHT41 - CO2, Temperature & Humidity Sensor - STEMMA QT / Qwiic. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/6478

### Description

CO₂ sensors are essential for determining if a room is too 'stuffy' - high CO₂ makes humans grumpy and tired. That's why it's always nice to take a deep breath outside where CO₂ is about 400 ppm. However, until now, CO₂ sensors were always really chunky ([like the SCD-30](https://www.adafruit.com/product/4867)) or pricey ([like the SCD-40](https://www.adafruit.com/product/5187)). [Inexpensive sensors like the SGP30 approximate the CO₂ using VOC gas concentration](http://www.adafruit.com/product/3709), but they don't actually measure CO₂.

The STCC4 is a tiny (4 x 3 x 1.2mm) sensor that can measure CO₂ gas and fit in just about any enclosure. It uses thermal conductivity (TC) instead of NDIR or photoacoustic measurements. TC is based on the inherent thermal conductivity of all gases. With a thorough understanding of the gas composition in ambient environments, subtle changes in gas concentrations can be detected. The measurement principle is based on heating the air within a measurement cavity and sensing the heat transfer with a temperature sensor. [For more details check out the EYE ON NPI video we did on this sensor!](https://www.youtube.com/watch?v=5mJqpmBHUV0)

The trade-off for the small size and lower cost is that STCC4 is that it's really tuned just for indoor air measurement applications - not for scientific CO₂ sensing or where the air gas composition is 'abnormal'. That said, the vast majority of use cases we see are indoor air monitoring to reduce illness and stuffiness and for that purpose the STCC4 is great!

One thing to note, like all true CO₂ sensors, it must be self-calibrated by having it exposed to outdoor air once a week, to get a baseline 400 ppm measurement - in practice that means opening a window or making sure fresh air gets to the sensor.

To round the STCC4 out and make it a perfect nini indoor air quality sensor, [we've added an SHT41 as well](https://www.adafruit.com/product/5776) to improve the CO₂ measurements. The SHT41 has an excellent ±1.8% typical relative humidity accuracy from 25 to 75% and ±0.2 °C typical accuracy from 0 to 75 °C. Note it is connected to the secondary I2C port on the STCC4 so that you only have to query the STCC4 to get measurements rather than talk to both chips with two libraries.

Such a lovely pair of chips - so we spun up a breakout board with the STCC4 + SHT41 and some supporting circuitry such as pullup resistors and capacitors. To make things even easier, we've included [SparkFun Qwiic](https://www.sparkfun.com/qwiic) compatible [STEMMA QT](https://learn.adafruit.com/introducing-adafruit-stemma-qt) connectors for the I2C bus so you don't even need to solder! [QT Cable is not included, but we have a variety in the shop](https://www.adafruit.com/?q=stemma+qt+cable&sort=BestMatch). 

If you prefer working on a breadboard, each order comes with one fully assembled and tested PCB breakout and a small piece of header. You'll need to solder the header onto the PCB, but it's fairly easy and takes only a few minutes even for a beginner.

We've written both Arduino and CircuitPython/Python library code for this chip, so you can use it with just about any microcontroller or single-board computer like Raspberry Pi.

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
