<h1> Lora Rain Sensor <h1>
  
  <h2> Hardware</h2>
   
 <p> There are different ways to get the hardware of the RoRa RainSensor.The most convenient one is to buy the whole device ready to use.You can still reflash and change the firmware. Source of th complet device for 69 EU is <a href="www.aqua-scope.com"> Aqua-Scope Technologies </a> </p>
  
  <h2> DIY Parts</h2>
  
  <p> If you want to built your own device, here is what you need </p>
  <table>
    <tr><td> Part</td><td>Source</td></tr>
    <tr><td> Main Enclosure <i>(incl. magic eye,package,screws)</i></td><td>Source, 14 &euro;</td></tr>
    <tr><td> Main PCB <i>(for own productionsee below)</i></td><td>Source, 18 &euro;</td></tr>
    <tr><td> 2 * AAA Battery <i> (We recommend VARTA Industrial Pro) </i></td><td>several Online Shops 0.60 ...1.00 &euro;</td></tr>
    <tr><td> Lora 868 MHz Antenna MOLEX  211140-0100  Antenne, ISM, 902MHz bis 928MHz </td><td> <a href="https://de.farnell.com/molex/211140-0100/ism-antenne-902-928mhz-1dbi/dp/3498957"> Farnell</a> 1.95 &euro;</td></tr>    
  </table>
  
 <h2> PCB Manufacturing</h2>
  
  <p> If you want to make your own PCB, in the folder /pcba you find the complete gerber files plus Bill of Material and Placement files for JLCPSB production.if you use <a href='http://www.jlcpcb.com'> this link </a>to order from JLCPCB we will receive 5 % of your pure PCB value (about 10 ct) per order as donation. </p>
  <p> The JLCPCB project contains the board without Reed Contact, RAK 3172 LPWAN Module and wires to connect to batery holder of the enclosure. You can order the PCB without assemlby only or ask JLCPCB to add the smaller components already to the board. JLCPCb minimum order quantity are 5 PCBS.Prices for the PCBs are </p>
   <ul>
      <li> 5 * raw PCB: 4 USD </li>
      <li> 5 * raw PCB incl shippment: 11 USD </li>
      <li> 5 * PCBA without RAK/Reed: 38 USD </li>
      <li> 5 * PCBA without RAK/Reed: 78 USD </li>
  </ul>
  
  <p> The missing components are available here</p> 
 
  <table>
  <tr><td> Part</td><td>Source</td></tr>  
  <tr><td> Reed Switch 59170-1-S-00-D</td><td>1.09 &euro; plus shippment from <a href="https://de.farnell.com/littelfuse/59170-1-s-00-d/reed-schalter-spst-no-6-5mm-10w/dp/2774139">Farnell</a> </td></tr>
<tr><td> RAK3172 WisDuo LPWAN Module </td><td>5,99 USD / 30.36 USD with shippment from <a href="https://store.rakwireless.com/products/wisduo-lpwan-module-rak3172"> RAK Online Store</a></td></tr>      
  </table>
  </table>  
  <h2> Firmware </h2>
  
  <p> The firmware is written als Arduino Sketch using the RAK Wireless Arduino Environment </p> You need to install the Arduino IDE and follow the instructions of <a href="https://docs.rakwireless.com/Product-Categories/WisDuo/RAK3172-Module/Quickstart/#rak3172-as-a-stand-alone-device-using-rui3"> RAK wireless </a> to install the RAk board support package. </p>
  
  <p> To flash the nw firmware you need a simple USB-TTLUART connector. Firmare update mode on the RAK module is enabled using the AT command 'AT+BOOT' on the swrial console of the Arduino IDE. </p>
  
