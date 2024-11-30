# ESP32-Framework
Since seriously getting into Arduino (thank you Joe) and ESP32 on retiring in 2020 I made a plan to stay at it as a means of keeping the brain ticking over. After all if you can write a chunk of code and get it debugged and running reliably then it's worth getting up the next day - and anyway a better option than going down to the day centre to do basket weaving.

As Scott Adams said around 25 years ago we're all getting more stupid. Not necessarily because we are, but because the technology we face is getting more complicated. By implication if I can do this year what I could do last year in the coding space then I've actually got more intelligent which is comforting.

Over the 4 years I have dabbled with matrix keypads, 4 line displays, Bluetooth etc, but finally settled on MQTT and Json as the cool way of doing things.
The very useful IoT MQTT Panel by Rahul Kundu has proved an excellent tool for building up the display and control ware for both local and cloud based use.
Out of all of this I have distilled what I call my base framework. Its the starting point for every new app and contains all the useful elements you see in the code comments. The key thing was to make it work slickly with WinMerge so all the code bases can be kept in sync.

Also a key part of the way-I-go-about-it code wise is keep it straight forward enough to get back into after maybe months and not needing piles of comments as these never stay up to gate. I do my {} the way I do as in Algol 60 from my Burroughs mainframe days the 'begin' was always on the next line for easy reading. And hopefully it will annoy the purists.

There is a bundle of stuff in there: Serial console, telnet, wifi, mqtt, time, restart error checking, properties.

At a system level there are three dedicated ESP32s: MQTTBroker, MQTTBridge to Hive, Telnet bridge from the cloud. All built off the framework. And then there are the apps actually doing useful things.

Enjoy. 
