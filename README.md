# MiningCore Web-UI
<h4>Miningcore WebUI for the Miningcore Pool</h4>

Miningcore is one of the best open source minning pools there are.
To make this pool look good, you have to have a nice and fast user interface.
MiningCore Web-UI does that for you and it is open source. so you can change it to suit your needs. 

How to Install & Configure
This Miningcore WebUI needs a working Miningcore Pool API
- Download the MiningCore Web-UI files
- Save them on your webserver and point your webserver config to the index.html.
  
You should now see the site and live pool API info:
  
<b>Website is visible, but no live data is shown</b></br>
Live info data is retrieved from the miningcore pool API.</br>
The WebUI website default looks at the domain-name/api.</br>
If this is not your api location, you need to edit the miningcore.js file.</br>

Chang API location</br>
- open the WebUI config file in you editor: js/miningcore.js
- change the following:

var WebURL         = window.location.protocol + "//" + window.location.hostname + "/";</br>
var API            = WebURL + "api/";</br>
var stratumAddress = "stratum+tcp://" + window.location.hostname + ":";</br>


It should look like this:</br>
(replace domain-name.com to your own domain name)</br>
var WebURL = "https://domain-name.com/";</br>
var API = "https://domain-name.com/api/";</br>
var stratumAddress = "stratum+tcp://domain-name.com"

<b>Suggestion</b></br>
Do you have an idea on what to add to the website, or you found a bug,
let me know and we will see what we can do.

<b>Features</b>
Multiple coins.
Miner Adjustable payout.

<b>Changes:</b></br>
Version 1.5  (08/08/2024)
- simple and fast WebUI (html and javascript)
- one file website displays selected info block and hides the rest
- one modern colorful look 


