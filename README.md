# DNSReaper


https://github.com/user-attachments/assets/543a4528-9efa-47af-9d12-b811b03b2eb5


☠️ Anonymous DNS Checker ☠️ 

A powerful DNS scanning tool designed for discovering and verifying DNS servers across various protocols. Whether you want to check DNS over UDP, TCP, or explore encrypted DNS protocols like DNS over HTTPS and DNS over TLS, this tool has you covered.

This tool offers a fast, parallel DNS scanning mechanism that can handle large-scale network scans with ease. It supports both file-based scanning and individual IP address checks, saving the results for future analysis.

✨ Command Breakdown: 1. Scan All Supported Ports: -scan 

What it does:
This command scans all supported DNS ports across the provided IP addresses or CIDR ranges. It checks DNS availability over various protocols including UDP 53, TCP 53, DNS over HTTPS (443), and DNS over TLS (853).



# usage

1. Clone the repository:

   ```bash
   git clone https://github.com/MrPYTHONI/DNSReaper.git
   cd DNSReaper
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the tool:

![Screenshot_20250209-070404_Termux](https://github.com/user-attachments/assets/2d70d68a-3eff-49d0-8123-eb2ece5db88a)


   ```bash
   python DNSReaper.py [IP_INPUT] [OPTIONS]
   ```

```bash
   python DNSReaper.py -f ipv4testdns.txt -scan
 ``` 

Description:

This will initiate a scan of all supported DNS protocols from the file ipv4testdns.txt. It will connect to each IP or CIDR range and test each protocol. The results are saved in the output file. 

What happens:
It will reveal which DNS servers are alive and working across the various protocols, showing the result in real-time in a bold and vibrant format.

2. Single IP Scan: -rn 

What it does:
This command allows you to scan a single IP address or CIDR range to check the availability of DNS servers over a specific port.

Usage:

```bash
   python DNSReaper.py -rn 192.168.1.1 -p "TCP 53"
```

Description:

Scans the specific IP 192.168.1.1 for DNS availability over TCP 53. You can either pass a single IP, a CIDR block, or a file with a list of IPs for the scan. 

What happens:

If the DNS is reachable, it will save the working result to the output file and notify you with a success message. You can specify the port (-p) you want to scan (for example, UDP 53, DNS over HTTPS, or others). 3. File Input: -f 

What it does:
This option lets you input a file that contains a list of IP addresses or CIDR ranges for batch scanning.

Usage:

   ```bash
   python DNSReaper.py -f yourfile.txt 
   ```

Description:

The tool will read the IPs or CIDR ranges from the file and start scanning them across all supported ports. The file should contain one IP or CIDR per line. If the file does not exist, you’ll be alerted with an error message. 

What happens:
This is a key feature for bulk scanning, especially useful for network administrators and security researchers who need to scan a large number of IP addresses or networks for DNS availability.

4. Port Selection: -p 

What it does:
This option allows you to select which DNS port you wish to scan for each IP or CIDR range.

Usage:

  ```bash
   python DNSReaper.py -rn 192.168.1.1 -p "DNS over HTTPS"
   ```
Description:

You can specify the exact protocol and port. The supported ports are: UDP 53: Traditional DNS over UDP. TCP 53: DNS over TCP. DNS over HTTPS (443): Encrypted DNS using HTTPS. DNS over TLS (853): Encrypted DNS using TLS. 

What happens:

The tool will check the specific DNS protocol and port for availability on the provided IP and will display the results in your terminal. 5. Output File: -o 

What it does:
This option specifies the output file where you want to save the working DNS servers that were found during the scan.

Usage:

```bash
   python DNSReaper.py -f ipv4testdns.txt -o results.txt
```

Description:

Results will be saved in the file you specify (results.txt). Only working DNS servers will be saved. This allows you to keep a record of your successful scans. 

What happens:

A list of working DNS servers will be written to the output file, with each entry showing the IP and the port used. 🔥 Tool Features: Multi-Protocol Support: Scan using UDP, TCP, DNS over HTTPS, and DNS over TLS. Bulk Scanning: Scan a list of IP addresses or CIDR ranges in parallel for faster results. Real-Time Updates: View the status of each IP as it’s being scanned, with working results saved immediately. Custom Output: Specify where to save the working DNS servers, keeping your data organized. 💀 Sample Output: 

If the DNS server is working and available:

[✔] 192.168.1.1 | TCP 53 WORKING ---> Saved 

If the DNS server is not working:

[✘] 192.168.1.1 | TCP 53 NOT WORKING ⚠️ Important Notes: Make sure the input file is formatted correctly, with one IP or CIDR per line. The tool will check for DNS servers over all supported ports by default unless specified otherwise. 🛠️ Example Commands: 

Scan a file with multiple IPs and save results:

```bash
   python dns_checker.py -f ipfile.txt -o working_dns.txt -scan 
 ```

Check a single IP for DNS availability over TCP 53:

```bash
   python dns_checker.py -rn 192.168.1.1 -p "TCP 53" -o result.txt
 ```

This tool is perfect for penetration testers, network administrators, and anyone involved in cybersecurity who needs to assess DNS server availability and security across various protocols.

☠️ Stay anonymous. Stay safe. MrPYTHON ☠️

```bash
Telegram 🏴‍☠️ :-
```
https://t.me/PYT_HON3

```bash
Welcome to our fun and dark gathering. We are happy to have you join our channel to benefit and not to mention more. Thank you!🏴‍☠️
```
```bash
Official Developer ⚙ :- 
MrPYTHON 🇾🇪
```
All my calculations :-

https://mrpython3.carrd.co/

My private id Tgileram to communicate :-

https://t.me/FPI_711



