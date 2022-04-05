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


## <font color=Crimson>Wireshark_DNS</font>  
![1.](https://github.com/RiverUp/networkTR/blob/main/DNS1.1.png)  
![2.](https://github.com/RiverUp/networkTR/blob/main/DNS1.2.png)  
![3.](https://github.com/RiverUp/networkTR/blob/main/DNS1.3.png)  
1. I looked up Baidu, its IP address is 36.152.44.96 and 36.152.44.95  
2. I looked up Oxford University
3. I used dns0.ox.ac.uk to query yahoo but failed, so I retried facebook and succeeded.  
   
![4.](https://github.com/RiverUp/networkTR/blob/main/DNS1.4.png)  
![5.](https://github.com/RiverUp/networkTR/blob/main/DNS1.5.png)  
![6.](https://github.com/RiverUp/networkTR/blob/main/DNS1.6.png)  
![7.](https://github.com/RiverUp/networkTR/blob/main/DNS1.7.png)  
![8.](https://github.com/RiverUp/networkTR/blob/main/DNS1.8.png)  
4. UDP  
5. Both are 53  
6. The DNS query message was sent to 202.114.96.1
   Yes, they are the same.
7. Type is A. And it didn't get any answer. 
8. It provided 3 answers. They contained ServerName, Type, Class, Time to live, Date length and Cname.  
9. No, they had no corresponce.  
10. No.
![11.](https://github.com/RiverUp/networkTR/blob/main/DNS1.11.png)  
![12.](https://github.com/RiverUp/networkTR/blob/main/DNS1.12.png)        
11. Both are 53.
12. The DNS query message was sent to 202.114.96.1  
   Yes, they are the same.  
13. The type is AAAA. And it got no answer.  
14. Two. They contained ServerName, Type, Class, Time to live, Date length and Cname.  
![13.](https://github.com/RiverUp/networkTR/blob/main/DNS1.13.png)    
![14.](https://github.com/RiverUp/networkTR/blob/main/DNS1.14.png)  
16. The DNS query message was sent to 202.114.96.1
   Yes, they are the same.  
17. The type is NS. And it had no answer.  
18. ns7.dnsmadeeasy.com
    ns6.dnsmadeeasy.com  
    ns5.dnsmadeeasy.com  
    atalante.stanford.edu  
    avallone.stanford.edu
    argus.stanford.edu  
    No, it didn't provide.  
![15.](https://github.com/RiverUp/networkTR/blob/main/DNS1.15.png)  
![16.](https://github.com/RiverUp/networkTR/blob/main/DNS1.16.png)  
20. It was sent to 171.64.7.115. They seemed to have no corresponce.  
21. The type is A. It didn't contain any answer.  
22. One. They contained ServerName, Type, Class, Time to live, Date length and Cname.  

## <font color=Crimson>Wireshark_UDP</font>    
1. There are 4 fields and they are Source Port, Destination Port, Length and Checksum.   
   ![udp1](https://github.com/RiverUp/networkTR/blob/main/udp1.png)  
2. There are four header fields and each of them occupies 2 bytes. So, totally, its length is 8 bytes.  
3. It is the length of header fields plus data fields.  
   ![udp2](https://github.com/RiverUp/networkTR/blob/main/udp2.png)
4. Length has 2 bytes so it can represent $ 2^{8*2} $ bytes data. And the header occupies 8. So, its maximum number is $ 2^{16}-8 $  
5. The Port also has 2 bytes. And the port number begins with 0. So, the largest is $ 2^{16}-1 $  
6. As the picture above shows, its 17. And Hexadecimally, it's 0X11  
7. Their Source Port is corresponding with the other Destination Port.