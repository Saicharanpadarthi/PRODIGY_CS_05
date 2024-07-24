# PRODIGY_CS_05

Here is a sample README file for the network packet analyzer:

---

# Network Packet Analyzer

A simple network packet analyzer that captures and prints information about IP packets using Scapy.

## Features

- Captures and displays the source and destination IP addresses of each packet.
- Identifies and prints protocol-specific information for TCP, UDP, and ICMP packets.
- Easy to use with minimal setup required.

## Requirements

- Python 3.x
- Scapy

## Installation

1. **Clone the repository:**

    ```sh
    git clone https://github.com/yourusername/network-packet-analyzer.git
    cd network-packet-analyzer
    ```

2. **Install the required Python packages:**

    ```sh
    pip install -r requirements.txt
    ```

3. **Ensure you have the necessary permissions to capture packets. You might need to run the script with elevated privileges (e.g., using `sudo` on Unix-based systems).**

## Usage

1. **Run the packet sniffer:**

    ```sh
    sudo python packet_sniffer.py
    ```

2. **The script will start capturing packets and display information about each packet in the console.**

## Example Output

```
Starting packet sniffer...
[+] New Packet: 192.168.1.2 -> 93.184.216.34
    Protocol: 6
    TCP Payload: <Raw  load='\x16\x03\x01\x00\x8f\x01\x00\x00\x8b\x03\x03TO\xf5T\xbc\xb9\xae\xa3t\xb2\xef\x93'...>

[+] New Packet: 192.168.1.2 -> 8.8.8.8
    Protocol: 17
    UDP Payload: <DNS  id=6507 qr=0 opcode=QUERY rd=1 qdcount=1 ancount=0 nscount=0 arcount=0 qd=<DNSQR  qname='www.google.com.' qtype=A qclass=IN |> |

[+] New Packet: 192.168.1.1 -> 192.168.1.2
    Protocol: 1
    ICMP Payload: <Raw  load='\x08\x00\xf7\xff\x00\x01\x00\x62'...>
```

## Acknowledgements

- [Scapy](https://scapy.net/) - the Python library used for packet manipulation.

## Contributing

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch`.
3. Make your changes.
4. Commit your changes: `git commit -m 'Add some feature'`.
5. Push to the branch: `git push origin feature-branch`.
6. Submit a pull request.

## Contact

For any questions or suggestions, feel free to open an issue or contact me directly.

---

Feel free to customize this README file further to suit your specific needs.
