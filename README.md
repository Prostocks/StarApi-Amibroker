# StarApi-Amibroker

Note: Works with Amibroker 64 bit only.

Instructions: 

1. Copy the ProStocksStar_x64.dll to Amibroker/Plugins folder
2. Copy cpprest141_2_10.dll to Amibroker folder

First Time:
1. Enter Login Credentials provided in the Credentials window. 

Place Order:
In your afl call the method when you want to send the signal to Star

NorenPlaceOrder(exch, tsym, qty, prc, trgprc, dscqty, prd, trantype, prctyp, ret, remarks);       

For eg:
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
	
