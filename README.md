# StarApi-Amibroker

Note: 


Instructions ( for 64 bit Amibroker): 

1. Copy the ProStocksStar_x64.dll to Amibroker/Plugins folder
2. Copy cpprest141_2_10.dll to Amibroker folder

Instructions ( for 32 bit Amibroker): 

1. Copy the ProStocksStar.dll to Amibroker/Plugins folder
2. Copy cpprest141_2_10.dll to Amibroker folder


First Time:
1. Enter Login Credentials provided in the Credentials window. 

Place Order:
In your afl call the method when you want to send the signal to Star

Logs:
AMIAPI_RequestLog.txt is created in Amibroker directory. Check the same for confirmations. 

NorenPlaceOrder(exch, tsym, qty, prc, trgprc, dscqty, prd, trantype, prctyp, ret, remarks);       

****
## Example
````
exch = "NSE";
tsym = "ACC-EQ";
qty = "1";
prc = Close;
trgprc = "0";
dscqty = "0";
trantype = "B";
prctyp = "L";
ret = "DAY";
remarks = "1234";
NorenPlaceOrder(exch, tsym, qty, prc, trgprc, dscqty, prd, trantype, prctyp, ret, remarks);       
````
