# Lab Report:  



## <font color=Crimson>Ping Another Computer </font>   
### 1.Abstract  
We are supposed to use our own computer to ping another one,and check the results.    
### 2.Introduction   
We are supposed to try using our own computer to ping another one. And in this practical way, we will know something about ping and computer network.  
### 3.Method  
#### Material:  
Two computers  
#### Procedure:  
1. Open my computer's hotspot and make another computer connect it.
2. Check the second computer's IP address.
3. Open my computer's command line and input the ping instruction.
4. check the result if the second comuper receive the data package.  
### 4.Result  
![ping's result](https://github.com/RiverUp/networkTR/blob/main/Snipaste_2022-02-16_21-13-42.png "ping's result")  
The second computer successfully received the package.  
### 5.Conclusion  
By using hotspor to connect two computers, their communication is successful.



## <font color=Crimson>Tracert a Server</font>  
### 1.Abstract  
We are supposed to use our own computer to tracert a server,and check the results.     
### 2.Introduction  
We are supposed to try using our own computer to tracert a server. And in this practical way, we will know something about tracerting and computer network.  
### 3.Method  
#### Material:  
Two computers  
#### Procedure:  
1. Open my computer's hotspot and make another computer connect it.
2. Check the second computer's DNS server.
3. Open my computer's command line and input the tracert instruction.
4. check the result
### 4.Result
![tracert's result](https://github.com/RiverUp/networkTR/blob/main/Snipaste_2022-02-16_21-14-59.png "travert's result")  
The result shows the second computer's DNS server is my own computer.It's successful.  
### 5.Conclusion  
By using hotspot to connect two computers, the computer sharing the hotspot is the DNS server of the other one.  



## <font color=Crimson>WireShark Introduction</font>
### 1.Abstract  
We are supposed to learn some basic skills about using WireShark by visiting college website  
### 2.Introduction
We are supposed to learn some basic skills about using WireShark by visiting college website 
### 3.Method
#### Material:
A computer connected with the Internet with a browser and WireShark  
#### Procedure:  
1. Start WireShark. Choose WLAN input and start capturing.
2. Open the browser and in the browser address bar, type http://cs.whu.edu.cn/.
3. After http://cs.whu.edu.cn/index.aspx pages can be rendered by the browser, stop capturing in the WireShark.
4. Check the list of captured packets select the message we need.
### 4.Result
![Introduction result](https://github.com/RiverUp/networkTR/blob/main/httpIntroduction2.png "WireShark Introduction's result")  
![Introduction's result](https://github.com/RiverUp/networkTR/blob/main/httpIntroduction1.png "WireShark Introduction's result")   
![Introduction's result](https://github.com/RiverUp/networkTR/blob/main/httpIntroduction3.png "WireShark Introduction's result")   
### 5.Conclusion  
1. As shown in Figure One
2. 0.551509s
3. cs.whu.edu.cn's ip:202.114.64.41  
   My ip:10.133.183.40
4. *[GET](https://github.com/RiverUp/networkTR/blob/main/wireshark_WLANG6DMI1.pdf )*   
   *[OK](https://github.com/RiverUp/networkTR/blob/main/wireshark_WLANG6DMI2 )*   



## <font color=Crimson>Telnet a website</font>
### 1.Abstract  
Telnet two websites  
### 2.Introduct  
We are supposed to telnet websites and sent *GET* message.  
### 3.Method 
#### Material:  
A computer.  
#### Procedure:  
1. Open Powershell and input the instruction `telnet mail.hust.edu.cn 25`  
2. Input the instruction `telnet cs.hust.edu.cn 80`  
3. After we connect the server, input the instruction  
   `GET /index.htm HTTP/1.1`  
   `host:cs.hust.edu.cn`  
### 4.Result  
![Introduction result](https://github.com/RiverUp/networkTR/blob/main/Snipaste_2022-03-05_23-03-57.png "telnet's result")  
![Introduction result](https://github.com/RiverUp/networkTR/blob/main/Snipaste_2022-03-05_23-02-52.png "telnet's result")  
### 5.Conclusion  
If we connect a server successfully via telnet instruction, we can sent GET request to the server and get the response.



## <font color=Crimson>Wireshark_HTTP</font>  
### Abstract
Use Wireshark to capture the packages while communicating via http, and get the information.  
### Introduction  
We capture the http packages of different types and we find out the details of these transmissions.  
### Method    
#### 1. The Basic HTTP GET/response interaction  
##### Procedure  
1.	Start up your web browser.
2.	Start up the Wireshark packet sniffer, but don’t yet begin packet capture.  Enter “http” (just the letters, not the quotation marks) in the display-filter-specification window and press enter, so that only captured HTTP messages will be displayed later in the packet-listing window.  (We’re only interested in the HTTP protocol here, and declutter all other uninteresting captured packets). 
3.	Wait a bit more than one minute (we’ll see why shortly), and then begin Wireshark packet capture.
4.	Surf website http://gaia.cs.umass.edu/wireshark-labs/HTTP-wireshark-file1.html in your browser
5.	Your browser should display a very simple, one-line HTML file.
6.	Stop Wireshark packet capture.
##### Result  
![http result](https://github.com/RiverUp/networkTR/blob/main/Inkedwireshark_http_LI.jpg) 
![http result](https://github.com/RiverUp/networkTR/blob/main/Inkedwireshark_http1_LI.jpg) 
![http result](https://github.com/RiverUp/networkTR/blob/main/Inkedwireshark_http2_LI.jpg)  
1. Both are HTTP 1.1   
2. zh-CN,zh  
3. my computer: 10.133.157.108  
   gaia.cs.umass.edu server: 128.119.245.12  
4. 200 
5. Sat, 12 Mar 2022 06：59: 01 GMT  
6. 128  
7. No.  
#### 2. The HTTP CONDITIONAL GET/response interaction  
##### Procedure  
•	Start up your web browser, and make sure your browser’s cache is cleared, as discussed above.
•	Start up the Wireshark packet sniffer
•	Enter the following URL into your browser
http://gaia.cs.umass.edu/wireshark-labs/HTTP-wireshark-file2.html
Your browser should display a very simple five-line HTML file. 
•	Quickly enter the same URL into your browser again (or simply select the refresh button on your browser)
•	Stop Wireshark packet capture, and enter “http” in the display-filter-specification window, so that only captured HTTP messages will be displayed later in the packet-listing window.  
##### Result  
![http result](https://github.com/RiverUp/networkTR/blob/main/wireshark_http3.png)  
![http result](https://github.com/RiverUp/networkTR/blob/main/Inkedwireshark_http4_LI.jpg)  
![http result](https://github.com/RiverUp/networkTR/blob/main/Inkedwireshark_http5_LI.jpg)  
![http result](https://github.com/RiverUp/networkTR/blob/main/Inkedwireshark_http6_LI.jpg)  
8. No  
9. Yes. There is content length.  
10. Yes. The time the web page was last modified  
11. 304, Not Modified. No.  
#### 3. Retrieving Long Documents  
##### Procedure  
•	Start up your web browser, and make sure your browser’s cache is cleared, as discussed above.
•	Start up the Wireshark packet sniffer
•	Enter the following URL into your browser
http://gaia.cs.umass.edu/wireshark-labs/HTTP-wireshark-file3.html
Your browser should display the rather lengthy US Bill of Rights.
•	Stop Wireshark packet capture, and enter “http” in the display-filter-specification window, so that only captured HTTP messages will be displayed. 
##### Result  
![http result](https://github.com/RiverUp/networkTR/blob/main/Inkedwireshark_http7_LI.jpg)  
![http result](https://github.com/RiverUp/networkTR/blob/main/Inkedwireshark_http8_LI.jpg) 
![http result](https://github.com/RiverUp/networkTR/blob/main/wireshark_http9.png)  
12.  One  
13.  No.53  
14.  200, OK  
15.  Five
#### 4. HTML Documents with Embedded Objects
##### Procedure  
•	Start up your web browser, and make sure your browser’s cache is cleared, as discussed above.
•	Start up the Wireshark packet sniffer
•	Enter the following URL into your browser
http://gaia.cs.umass.edu/wireshark-labs/HTTP-wireshark-file4.html
Your browser should display a short HTML file with two images. These two images are referenced in the base HTML file.  That is, the images themselves are not contained in the HTML; instead the URLs for the images are contained in the downloaded HTML file. As discussed in the textbook, your browser will have to retrieve these logos from the indicated web sites.   The textbook publisher’s logo is retrieved from the gaia.cs.umass.edu web site.  The image of the cover for the 5th edition of the textbook is stored at the caite.cs.umass.edu server. (These are two different web servers inside cs.umass.edu).
•	Stop Wireshark packet capture, and enter “http” in the display-filter-specification window, so that only captured HTTP messages will be displayed. 
##### Result  
![http result](https://github.com/RiverUp/networkTR/blob/main/Inkedwireshark_http9_LI.jpg) 
16. Three  
17. According to the order of the respones, I guess its serial. 