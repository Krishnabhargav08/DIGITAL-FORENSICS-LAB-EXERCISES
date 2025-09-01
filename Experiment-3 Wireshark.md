# Experiment 3: Password Capturing Using Wireshark

## Aim
To capture and analyze network packets using Wireshark.

## Requirements
- Wireshark
- Windows Operating System
- Active internet connection or local network traffic

## Description
- Wireshark captures network packets in real-time or from saved files, allowing detailed inspection of protocols, packet contents, and network traffic patterns.
- It supports thousands of network protocols, enabling analysis of everything from TCP/IP to VoIP, with detailed dissection of packet headers and payloads.

## Steps

### Step-1
Open the Wireshark, there you will see the different types of networks. Select the network that is connected to your network, in this case it is Wi-Fi.

![(images/step1.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/81e4b3ac1b4592b23df85c0793e4efb92ddd373d/images/Ex-3%20im1.png)

### Step-2
On the top right corner you will see blue shark fin, just press the button and Wireshark begins capturing live traffic packets appear in real-time.

![(images/step2.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/81e4b3ac1b4592b23df85c0793e4efb92ddd373d/images/Ex-3%20im2.png)

### Step-3
After starting the packet capturing we will go to the website and login the credential on that website.

![(images/step3.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/81e4b3ac1b4592b23df85c0793e4efb92ddd373d/images/Ex-3%20im3.png)

### Step-4
Now go to Wireshark tool and apply some filters like HTTP to find the HTTP packets on the network.

![(images/step4.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/81e4b3ac1b4592b23df85c0793e4efb92ddd373d/images/Ex-3%20im4.png)

### Step-5
So, there are some HTTP packets are captured but we 
specifically looking for form data that the user submitted to the 
website. We have main two methods used for submitting form 
data from web pages like login forms to the server. They are ‘GET’ 
& ‘POST’ 

### Step-6
So, firstly for knowing the credential we use the first method and apply the filter for the GET methods.  
http.request.method == “GET”

![(images/step5.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/81e4b3ac1b4592b23df85c0793e4efb92ddd373d/images/Ex-3%20im5.png)

### Step-7
Now after checking the GET method if we didn’t find the form data, then we will try the POST method for that we will apply the filter on Wireshark.  

http.request.method == “POST”

As you can see the HTML form just click that form you can see the user credentials like username and password.  

Form item: “uname” = “Krishna Bhargav”  

Form item: “pass” = “KRISHNA”

![(images/step6.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/81e4b3ac1b4592b23df85c0793e4efb92ddd373d/images/Ex-3%20im6.png)
