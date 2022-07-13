<h1> Lora Rain Sensor <h1>
  
  <h2> Hardware</h2>
   
 <p> There are different ways to get the hardware of the LoRa RainSensor. The most convenient one is to buy the whole device ready to use. You can still reflash and change the firmware. Source of the complete device for XXX EU is <a href="www.aqua-scope.com"> Aqua-Scope Technologies </a> </p>
  
  <h2> DIY Parts</h2>
  
  <p> If you want to make your own device, you can source the different components. Solder the reed contact to the back side of the PCBa plus connect VCC and GND to the battery holder of the enclosure. </p>
  <table>
    <tr><td> Part</td><td>Source</td></tr>
    <tr><td> Main Enclosure <i>(incl. magic eye, package, screws)</i></td><td>Source, 14 &euro;</td></tr>
    <tr><td> Main PCB <i>(for own production see below)</i></td><td>Source, 18 &euro;</td></tr>
   <tr><td> Reed Switch 59170-1-S-00-D</td><td>1.09 &euro; plus shipment from <a href="https://de.farnell.com/littelfuse/59170-1-s-00-d/reed-schalter-spst-no-6-5mm-10w/dp/2774139">Farnell</a> </td></tr>   
    <tr><td> 2 * AAA Battery <i> (We recommend VARTA Industrial Pro) </i></td><td>several Online Shops 0.60 ...1.00 &euro;</td></tr>
    <tr><td> Lora 868 MHz Antenna MOLEX  211140-0100  Antenna, ISM, 902MHz bis 928MHz </td><td> <a href="https://de.farnell.com/molex/211140-0100/ism-antenne-902-928mhz-1dbi/dp/3498957"> Farnell</a> 1.95 &euro;</td></tr>    
  </table>
  
 <h2> PCB Manufacturing</h2>
  
  <p> If you want to make your own PCB, in the folder /pcba you find the complete Gerber files plus Bill of Material and Placement files for <a href="https://www.jlcpcb.com">JLCPCB</a> production.  </p>
  <p> The JLCPCB project contains the board without Reed Contact, RAK 3172 LPWAN Module and wires to connect to battery holder of the enclosure. You can order the PCB without assembly only or ask JLCPCB to add the smaller components already to the board. JLCPCBs minimum order quantity are 5 PCBs. Prices for the PCBs are </p>
   <ul>
      <li> 5 * raw PCB: 4 USD </li>
      <li> 5 * raw PCB incl shipment: 11 USD </li>
      <li> 5 * PCBA without RAK module: 38 USD </li>
      <li> 5 * PCBA without RAK module: 78 USD </li>
  </ul>
  
  <p> The missing components are available here</p> 
 
  <table>
  <tr><td> Part</td><td>Source</td></tr>  
  
<tr><td> RAK3172 WisDuo LPWAN Module </td><td>5,99 USD / 30.36 USD with shipment from <a href="https://store.rakwireless.com/products/wisduo-lpwan-module-rak3172"> RAK Online Store</a></td></tr>      
  </table>
  </table>  
  <h2> Firmware </h2>
  
  <p> The firmware is written as Arduino Sketch using the RAK Wireless Arduino Environment </p>. You need to install the Arduino IDE and follow the instructions of <a href="https://docs.rakwireless.com/Product-Categories/WisDuo/RAK3172-Module/Quickstart/#rak3172-as-a-stand-alone-device-using-rui3"> RAK wireless </a> to install the RAK board support package. </p>
  
  <p> To flash a new firmware you need a simple USB-TTL-UART connector (<a href="https://www.amazon.de/AZDelivery-Konverter-kompatibel-Arduino-inklusive/dp/B089QJZ51Z/ref=asc_df_B089QJZ51Z"> e.g. this </a>). The firmware update mode on the RAK module is enabled using the AT command 'AT+BOOT' on the serial console of the Arduino IDE. </p>
  
