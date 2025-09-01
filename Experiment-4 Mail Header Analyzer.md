# Experiment 4: Analyze Email Headers and Detect Email Spoofing Using Mail Header Analyzer

## Aim
To analyze email headers and detect possible spoofing or malicious activity using Mail Header Analyzer.

## Requirements
- Mail Header Analyzer tool
- Any email client (Gmail/Outlook/Yahoo) with suspicious email samples

## Description
- A mail header analyzer tool is used to examine email headers, which contain metadata about an email’s origin, routing, and authentication details.
- Mail header analyzers parse complex email headers per RFC 822 standards, transforming technical data into a human-readable format, detailing sender, recipient, subject, timestamps, and server paths.

## Steps

### Step-1
First get the email header for that open the gmail, select the mail and click the three dots, choose the show original.

![(images/step1.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/a345dbee87f8098522dacc0210f61f9cac125193/images/Ex-4%20im1.png)

### Step-2
Click the show original then you will see the original message with sender and receiver details.

![(images/step2.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/a345dbee87f8098522dacc0210f61f9cac125193/images/Ex-4%20im2.png)

### Step-3
Use Mail Header Analyzer tool for easy reading and analysis.

![(images/step3.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/a345dbee87f8098522dacc0210f61f9cac125193/images/Ex-4%20im3.png)

### Step-4
Copy and paste the entire header text and click Analyze header.

![(images/step4.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/a345dbee87f8098522dacc0210f61f9cac125193/images/Ex-4%20im4.png)

### Step-5
Check for IP Addresses and Hostnames, use tools like WHOIS or online IP lookup services to identify the geographical location and ownership of the IP addresses found in the Received lines. Check if any IP addresses are suspicious or if the hostname does not match the expected sending server.

![(images/step5.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/a345dbee87f8098522dacc0210f61f9cac125193/images/Ex-4%20im5.png)

### Step-6
Examine the SPF, DKIM, and DMARC Results.

![(images/step6.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/a345dbee87f8098522dacc0210f61f9cac125193/images/Ex-4%20im6.png)

- **SPF - Sender Policy Framework**: Checks if the sender’s server/IP is allowed for that domain.
- **DKIM - DomainKeys Identified Mail**: Ensures email content wasn’t changed.

![(images/step6.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/a345dbee87f8098522dacc0210f61f9cac125193/images/Ex-4%20im7.png)

![(images/step6.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/a345dbee87f8098522dacc0210f61f9cac125193/images/Ex-4%20im8.png)
