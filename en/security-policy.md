## TOAST > TOAST Security Policy 

TOAST guides for security products, security policy, and vulnerability information, to provide safer security environment.
Security policy is provided as below, to protect customer's resources from new and various types of attacks and security vulnerabilities, and prepare against frequent accidents and threats in the cloud.

## Password Policy 
To set passwords for user accounts (both root and general accounts), general passwords that are easy to guess may be cracked by unauthorized users and obtain authority for general or root accounts and access systems. As this may result in the leakage of important data saved in the server or abused as hackers' stop, a safe password must be set and managed. .

### Safe Passwords
Must be comprised of 8 or more characters, in combination of alphabets, numbers, and special characters. Following passwords should be avoided as they are easy to guess: 

- null Passwords
- Comprised only of characters or numbers 
- Same as user ID 
- Consecutive characters or numbers (e.g: 1111, 1234, or adcd)
- Periodic reuses 
- Composed of phone number, birthday, account name, or host name, which are easy to guess 

### TOAST Password Policy 
To protect customer's resources and services, TOAST applies the following as the basic password policy.

- Combined with three types: Alphabets, Numbers, and Special Characters
- Has more than 8 characters

## Anti-DRDoS Policy
Instances exposed to external networks may be abused as stops for Distributed Reflection Denial of Service, or DRDoS attacks, causing service failure or unintentional traffic charges due to abnormal increase in outbound traffic. 

### What is DRDoS (Distributed Reflection Denial of Service)?
DRDoS occurs due to vulnerable settings of applications, such as DNS, NTP, SSDP, or Memcached. This bandwidth amplifying attack technique is widely used for recent hackings, as it creates a large response packet with small request packets by using a number of zombie computers, and causes traffic to be concentrated at a target server.

### Anti-TOAST DRDoS Port Policy
To protect customer's resources and services, TOAST blocks UDP ports which are frequently abused as stops for DRDoS attacks..

### List of Blocked Ports
|Service Name |  Blocked Port  | Blocking Method |Reference|
| ---- | ---- | ---- | ---- |
|Chargen | UDP / 19    | Network ACL | Inaccessible from outside |
|SSDP    | UDP / 1900  | Network ACL | Inaccessible from outside |
|Memcached   | UDP / 11211 | Network ACL | Inaccessible from outside |


## Internet Port Blocking Policy (Inbound) 
To protect customer service, the block-intrusion system is provided as well as security group which is managed under the control of customers.

### TOAST List of Blocked Ports 
|Region | Service Name | Blocked Port | Blocking Method | Remarks |
| ---- | ---- | ---- | ---- | ---- |
| Korea (Pangyo) <br> Japan (Tokyo) <br> US (California) | System Terminal Port | TCP/23 | Blocked by network ACLs | Externally inaccessible |

### How to Apply for More Ports
- Download the excel file below and fill in the form.

[![](http://static.toastoven.net/prod_gov_security/img_04.png)](http://static.toastoven.net/prod_gov_security/Application%20for%20Exception%20from%20TOAST%20Firewall%20and%20SSL%20VPN%20Policy_Agency%20Name.xlsx)

- Save file name as “Application for Exception from TOAST Firewall and SSL VPN Policy_JP-Agency Name.xlsx”.
Send the application over the email like below (to be processed and replied within 3 days after received). 
    - TOAST : support@toast.com
    - TOAST G : support@gov.toast.com
