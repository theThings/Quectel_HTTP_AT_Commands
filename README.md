# Quectel_HTTP_AT_Commands
AT Commands to connect Quectel M95 to thethings.iO Platform

Below you can find the commands shown on the Quectel M95 tutorial accessible on blog.thethings.io

## Test Command
AT <CR><LF>

### Step 1
AT+QIFGCNT=0<CR><LF>

### Step 2
AT+QICSGP=1,"airtelnet.es"<CR><LF> //Replace with your apn setting

### Step 3
AT+QHTTPURL=78,30<CR><LF>

### Step 4
https://api.thethings.io/v2/things/E4hAefnMbGy3hODTo7NzVJv_A5Tu1dz708OC2jRFEwU //Replace with your thingtoken

### Step 5
AT+QHTTPPOST=47,50<CR><LF>

### Step 6
{"values":[{"key":"Temperature","value":"25"}]}

### Step 7
AT+QHTTPREAD=30<CR><LF>
