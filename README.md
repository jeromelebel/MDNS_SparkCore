Changelog
=========

09/04/2014 - 1.1.0 
- API change : ip type changed from uint32_t to IPAddress - ip optional, set to local ip in that case.
- Update from deprecated Network API to new WiFi API.
- Compilation warnings removed.
- Source files renamed.
- Include paths changed to be used in the same directory than the user code.



Spark Core and MDNS (fork from krvarma repository)
-------------------

Here is the Spark Core port of Adafruit MDNS library. The library provides the ability to setup a name for the Spark Core and resolve it. We can name the Core anything we want, the library will append "**.local**" to the name and we can access the Core using the URL "*name*.local".

The sample application names the Core as "***myspark***". If the MDNS is setup correctly then it creates a TCPServer on port 80. The Core can be accessed using the URL "**http://myspark.local**". The server simply prints a test message.

**Requirement**

 1. For Mac OSX support is built in through Bonjour already. 
 2. For Linux, install Avahi. 
 3. For Windows, install Bonjour.
 
**Screenhots**

![enter image description here][1]


  [1]: https://raw.githubusercontent.com/krvarma/MDNS_SparkCore/master/screenshot.jpg