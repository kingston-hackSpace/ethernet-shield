<h1>Ethernet shield</h1>
<p>The Arduino Ethernet Shield is an additional circuit board that fits on top of a Arduino. It extends the Arduino's capabilities with circuitry to connect to a network router, using a commonly-available RJ45 Ethernet cable. Your Arduino projects can communicate with the world through this connection - everything form fetching information from the internet and displaying it on a LCD screen, to providing publicly accessible, web-based tools that can control motors or other hardware.</p>

<p>A good book that covers a lot of techniques is</p>
<link>http://amazon.com/arduino_ethernet</link>

<h2>Ethernet methods</h2>
<p>The Ethernet library contains the following methods</p>

```Ethernet.begin((uint8_t*)mac, (uint8_t*)ip);```
<p>Initiates the ethernet object, requires byte arrays for the mac address and the ip. These can be found on the reverse of the ethernet shield.</p>

```Ethernet.localIP()```
<p>Returns the local ip address</p>

```Ethernet.gatewayIP()```
<p>Returns the gatewayIP, this is the IP address for the router.</p>

```Ethernet.subnetMask()```
<p>Returns the subnetmask, this is to improve performance for communication over the local area network.</p>

```Ethernet.dnsServerIP()```
<p>returns the DNS server IP</p>

```EthernetServer myServer(80);```
<p>Creates the ethernet server object</p>

```EthernetClient myClient;```
<p>Creates the ethernet client object that can be called on later int he script.</p>

```myClient.print("MESSAGE HERE");```
<p>Send messages via the client</p>

<code>myClient.write("MESSAGE HERE");</code>
<p>Send data via the connection</p>

<code>myClient.read();</code>
<p>Get data from the connection</p>
