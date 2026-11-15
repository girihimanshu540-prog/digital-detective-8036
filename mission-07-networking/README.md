# Mission 7 — How Computers Communicate

## 1. Task / objective
network types and concepts,network lookup and
connectivity, and what happens when a website opens ?

## 2. Work completed
Explored all the network system .

### Task 7.1 — Network concepts

| Concept | In my own words | Example |
|---------|-----------------|---------|
| LAN | A network that connects devices in a small area, such as one home, lab or office, so they can share data and resources | The Wi-Fi network in my home or college lab |
| MAN | A network that covers a whole city or a large campus, linking several smaller networks together | A university's campus-wide network, or a city-wide cable network |
| WAN | A network that spreads across a large geographical area, such as between cities or countries | The internet |
| DNS | A system that translates a domain name that people can remember into the IP address that computers use | Typing a website name in the browser and DNS finding the server's IP address |
| Router | A device that connects different networks and forwards data between them so it reaches the right place | My home router connecting my devices to the internet |
| Protocol | A set of rules that devices follow so they can understand each other when they communicate | HTTPS for loading secure websites |
| Packet switching | Data is split into small packets that travel across the network separately and are put back together at the destination | A photo sent online as many small packets that are reassembled on the other side |
| Client-server | A client asks for a service and a server provides it | My browser (client) requesting a page from a website's server |

### Task 7.2 — Network observations

**Commands run:** `ping -c 4 example.com` and `nslookup example.com`

**What I observed:**
- `ping`: (Write whether replies came back and roughly how long they took. If it timed out, say so, because some networks block ping.)
- `nslookup`: (Write the IP address shown for example.com. Replace the DNS server lines at the top with [redacted].)

- **What a connectivity test helps check:** It checks whether my computer can reach another computer over the network, and how long the replies take. If replies come back, the connection works. If they don't, something between us is down or blocking the test.
- **What a DNS lookup displays:** It shows the IP address (the numeric network address) that belongs to a domain name.
- **The role of DNS when I enter a website name:** Computers find each other by IP address, not by names. When I type a website name, DNS translates it into the IP address of the server, so my browser knows where to send its request.

### Task 7.3 — What happens when I open a website
1. I type a website address into my browser, which acts as the **client**, and press Enter.
2. The browser asks **DNS** to translate the domain name into the IP address of the website's server.
3. The browser prepares a request using a **protocol**, usually HTTPS, which is the set of rules both sides follow to communicate.
4. The request is split into packets and travels from my device through my router and across the networks of the internet to the server.
5. The **server** receives the request, finds the page and prepares a response.
6. The response travels back to my computer as packets, which are put back together.
7. My browser reads the response and displays the web page on my screen.

## 3. Commands / tools used
`ping` and `nslookup` 

