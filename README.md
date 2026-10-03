Task 1 — Answers

Q1. What is the IP address of your DNS server? Is it public or private?

My DNS server is 172.20.10.1. It is a private IP address.

Q2. Which IP address did google.com resolve to? Did your partner get the same one? Why might they differ?
У тебя google.com вернул несколько адресов. Можно написать один IPv4:

Google.com resolved to 142.250.154.102. My partner may get a different IP address because Google has many servers in different locations.

Q3. Is your own laptop a DNS server? Explain in one sentence.

No, my laptop is not a DNS server because it uses 172.20.10.1 as its DNS server.


Task 2

Q1.
Email is delivered to gmail-smtp-in.l.google.com because it has the lowest MX preference number (5).

Q2.
The authoritative name servers are ns1.google.com, ns2.google.com, ns3.google.com, and ns4.google.com.

Q3.
The TXT records contain verification keys and an SPF record. They are used to verify the domain and protect email from unauthorized senders.

Q4.
I chose apec.edu.kz.
A record: 75.2.60.5
NS records: ns1.hoster.kz, ns2.hoster.kz, ns3.hoster.kz

Q5.
Screenshot of the CMD with at least two record types.

Task 3 — Be the Resolver

Q1. Draw the path you walked:

You → a.root-servers.net → a.gtld-servers.net → hera.ns.cloudflare.com → 104.20.23.154

Q2. How many servers did you ask before you got the final answer?

I asked 3 DNS servers before getting the final answer: the root server, the .com TLD server, and the authoritative server.

Q3. Why is there no single server that knows every domain in the world?

There is no single server because DNS is distributed between many servers. This makes DNS faster, more reliable, and easier to manage.

Q4. Bonus (Ubuntu):

I use Windows, so I did not complete this bonus task.


Task 4 

Q1. What was the TTL the first time? What happened when you checked again after 5–10 seconds?

The first TTL was 77 seconds for the A records. After 5–10 seconds, it decreased to 31 seconds because the cached record was getting closer to expiration.

Q2. What changed after flushing the cache?

After flushing the DNS cache, the cached DNS records were cleared. A new lookup was performed and the TTL was refreshed. The new TTL was 152 seconds for the A records and 155 seconds for the AAAA records.

Q3. Why would you set a short TTL before moving a website to a new server?

A short TTL makes DNS records expire faster. This helps users get the new server address sooner after the DNS record is changed.
