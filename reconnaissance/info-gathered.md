### Main Domain : www.paypal.com

## Passive Scans

`Dig www.paypal.com`

; <<>> DiG 9.20.22-1-Debian <<>> www.paypal.com
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 47014
;; flags: qr rd ra; QUERY: 1, ANSWER: 3, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 512
;; QUESTION SECTION:
;www.paypal.com.			IN	A

;; ANSWER SECTION:
www.paypal.com.		284	IN	CNAME	www.glb.paypal.com.
www.glb.paypal.com.	265	IN	CNAME	paypal-dynamic.map.fastly.net.
paypal-dynamic.map.fastly.net. 217 IN	A	146.75.33.21

;; Query time: 19 msec
;; SERVER: 75.75.75.75#53(75.75.75.75) (UDP)
;; WHEN: Sat May 23 09:58:08 WAT 2026
;; MSG SIZE  rcvd: 124

# Dig on subdomain

`i.paypal.com`

; <<>> DiG 9.20.22-1-Debian <<>> i.paypal.com
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 53936
;; flags: qr rd ra; QUERY: 1, ANSWER: 11, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 512
;; QUESTION SECTION:
;i.paypal.com.			IN	A

;; ANSWER SECTION:
i.paypal.com.		14	IN	CNAME	v120gszvrs.data.adobedc.net.
v120gszvrs.data.adobedc.net. 112 IN	A	63.140.38.107
v120gszvrs.data.adobedc.net. 112 IN	A	63.140.38.213
v120gszvrs.data.adobedc.net. 112 IN	A	63.140.38.116
v120gszvrs.data.adobedc.net. 112 IN	A	63.140.39.254
v120gszvrs.data.adobedc.net. 112 IN	A	63.140.39.87
v120gszvrs.data.adobedc.net. 112 IN	A	63.140.39.210
v120gszvrs.data.adobedc.net. 112 IN	A	63.140.39.154
v120gszvrs.data.adobedc.net. 112 IN	A	63.140.39.114
v120gszvrs.data.adobedc.net. 112 IN	A	63.140.39.244
v120gszvrs.data.adobedc.net. 112 IN	A	63.140.39.123

;; Query time: 15 msec
;; SERVER: 75.75.75.75#53(75.75.75.75) (UDP)
;; WHEN: Sat May 23 09:58:28 WAT 2026
;; MSG SIZE  rcvd: 242


` whois 146.75.33.21 `

#
# ARIN WHOIS data and services are subject to the Terms of Use
# available at: https://www.arin.net/resources/registry/whois/tou/
#
# If you see inaccuracies in the results, please report at
# https://www.arin.net/resources/registry/whois/inaccuracy_reporting/
#
# Copyright 1997-2026, American Registry for Internet Numbers, Ltd.
#


NetRange:       146.75.0.0 - 146.75.255.255
CIDR:           146.75.0.0/16
NetName:        RIPE-ERX-146-75-0-0
NetHandle:      NET-146-75-0-0-1
Parent:         NET146 (NET-146-0-0-0-0)
NetType:        Early Registrations, Transferred to RIPE NCC
OriginAS:       
Organization:   RIPE Network Coordination Centre (RIPE)
RegDate:        2004-02-04
Updated:        2025-02-10
Comment:        These addresses have been further assigned to users in the RIPE NCC region. Please note that the organization and point of contact details listed below are those of the RIPE NCC not the current address holder. ** You can find user contact information for the current address holder in the RIPE database at http://www.ripe.net/whois.
Ref:            https://rdap.arin.net/registry/ip/146.75.0.0

ResourceLink:  https://apps.db.ripe.net/db-web-ui/query
ResourceLink:  whois.ripe.net


OrgName:        RIPE Network Coordination Centre
OrgId:          RIPE
Address:        P.O. Box 10096
City:           Amsterdam
StateProv:      
PostalCode:     1001EB
Country:        NL
RegDate:        
Updated:        2013-07-29
Ref:            https://rdap.arin.net/registry/entity/RIPE

ReferralServer:  whois.ripe.net
ResourceLink:  https://apps.db.ripe.net/db-web-ui/query

OrgAbuseHandle: ABUSE3850-ARIN
OrgAbuseName:   Abuse Contact
OrgAbusePhone:  +31205354444 
OrgAbuseEmail:  abuse@ripe.net
OrgAbuseRef:    https://rdap.arin.net/registry/entity/ABUSE3850-ARIN

OrgTechHandle: RNO29-ARIN
OrgTechName:   RIPE NCC Operations
OrgTechPhone:  +31 20 535 4444 
OrgTechEmail:  hostmaster@ripe.net
OrgTechRef:    https://rdap.arin.net/registry/entity/RNO29-ARIN


#
# ARIN WHOIS data and services are subject to the Terms of Use
# available at: https://www.arin.net/resources/registry/whois/tou/
#
# If you see inaccuracies in the results, please report at
# https://www.arin.net/resources/registry/whois/inaccuracy_reporting/
#
# Copyright 1997-2026, American Registry for Internet Numbers, Ltd.
#



Found a referral to whois.ripe.net.

% This is the RIPE Database query service.
% The objects are in RPSL format.
%
% The RIPE Database is subject to Terms and Conditions.
% See https://docs.db.ripe.net/terms-conditions.html

% Note: this output has been filtered.
%       To receive output for a database update, use the "-B" flag.

% Information related to '146.75.0.0 - 146.75.255.255'

% Abuse contact for '146.75.0.0 - 146.75.255.255' is 'abuse@fastly.com'

inetnum:        146.75.0.0 - 146.75.255.255
netname:        FASTLY
descr:          FASTLY
geofeed:        https://ip-geolocation.fastly.com/
org:            ORG-FI26-RIPE
country:        SE
admin-c:        FRA59-RIPE
tech-c:         FRA59-RIPE
status:         LEGACY
mnt-by:         RIPE-NCC-LEGACY-MNT
mnt-by:         FASTLY
mnt-lower:      FASTLY
mnt-routes:     FASTLY
created:        2002-01-03T10:06:41Z
last-modified:  2022-02-11T15:12:28Z
source:         RIPE # Filtered

organisation:   ORG-FI26-RIPE
org-name:       Fastly, Inc.
country:        US
reg-nr:         4947714 (Delaware)
org-type:       LIR
address:        PO Box 78266
address:        94107
address:        San Francisco, CA
address:        UNITED STATES
phone:          +14157580146
mnt-by:         FASTLY
mnt-ref:        FASTLY
mnt-ref:        RIPE-NCC-HM-MNT
mnt-by:         RIPE-NCC-HM-MNT
abuse-c:        FAT25-RIPE
tech-c:         FRA59-RIPE
created:        2013-07-08T09:37:51Z
last-modified:  2026-05-13T07:15:00Z
source:         RIPE # Filtered
admin-c:        FRA59-RIPE

role:           Fastly RIR Administrator
org:            ORG-FI26-RIPE
address:        PO Box 78266
address:        San Francisco CA 94107
phone:          +1 (415) 404-9374
nic-hdl:        FRA59-RIPE
mnt-by:         FASTLY
created:        2014-09-24T14:49:45Z
last-modified:  2014-09-25T15:10:14Z
source:         RIPE # Filtered

% This query was served by the RIPE Database Query Service version 1.122.1 (ABERDEEN)


# *DNSRECON*

` dnsrecon -d paypal.com -D <wordlist> `

2026-05-23T10:28:49.883984+0100 INFO Starting enumeration for domain: paypal.com
2026-05-23T10:28:49.911985+0100 INFO std: Performing General Enumeration against: paypal.com...
2026-05-23T10:28:50.013042+0100 INFO DNSSEC is configured for paypal.com
2026-05-23T10:28:50.047020+0100 INFO DNSKEYs:
2026-05-23T10:28:50.047626+0100 INFO 	NSEC3 ZSK ECDSAP256SHA256 b7bff13dc7c29f352bc4a6b0b269d1f9 2c500094922c0041b7ecbb795dbf0729 69a86eaf846b89455192b077ae06dfd5 8c2e88072a953181aed49f7efecd506d
2026-05-23T10:28:50.048167+0100 INFO 	NSEC3 ZSK ECDSAP256SHA256 dafcb1db4411c9e5b5de6d039f39d9b0 0668853a91a94d67290de16c276c487c eed4eea57f0cc3584700446c9e35e5fa 9ee920b2841a0bf7fa008f90057d6202
2026-05-23T10:28:50.048641+0100 INFO 	NSEC3 KSk ECDSAP256SHA256 d4d62651e37f127b357399bc966ab9fd 28aa8e930af9d7c60d8fb78fc2a40e00 d288341ebf9f49971a5048881157bdb7 34606b339c320ed391676d2b495902a8
2026-05-23T10:28:50.129745+0100 INFO 	 SOA ppdns.paypal.com 64.78.206.1
2026-05-23T10:28:50.332687+0100 INFO 	 NS ns1-pchnet.paypal.com 64.78.206.1
2026-05-23T10:28:50.383679+0100 INFO 	 Bind Version for 64.78.206.1 "paypalbe"
2026-05-23T10:28:50.384265+0100 INFO 	 NS ns1-pchnet.paypal.com 2620:171:814:1701:2::1
2026-05-23T10:28:50.424090+0100 INFO 	 Bind Version for 2620:171:814:1701:2::1 "paypalbe"
2026-05-23T10:28:50.424673+0100 INFO 	 NS ns2-pchnet.paypal.com 64.78.207.1
2026-05-23T10:28:50.463871+0100 INFO 	 Bind Version for 64.78.207.1 "paypalbe"
2026-05-23T10:28:50.464435+0100 INFO 	 NS ns2-pchnet.paypal.com 2620:171:815:1701:2::1
2026-05-23T10:28:50.502072+0100 INFO 	 Bind Version for 2620:171:815:1701:2::1 "paypalbe"
2026-05-23T10:28:50.502614+0100 INFO 	 NS pdns100.ultradns.com 156.154.64.100
2026-05-23T10:28:50.538929+0100 INFO 	 Bind Version for 156.154.64.100 Nameserver"
2026-05-23T10:28:50.539506+0100 INFO 	 NS pdns100.ultradns.com 2001:502:f3ff::88
2026-05-23T10:28:50.576327+0100 INFO 	 Bind Version for 2001:502:f3ff::88 Nameserver"
2026-05-23T10:28:50.576588+0100 INFO 	 NS pdns100.ultradns.net 156.154.65.100
2026-05-23T10:28:50.618979+0100 INFO 	 Bind Version for 156.154.65.100 Nameserver"
2026-05-23T10:28:50.619551+0100 INFO 	 NS pdns100.ultradns.net 2610:a1:1014::88
2026-05-23T10:28:50.661004+0100 INFO 	 Bind Version for 2610:a1:1014::88 Nameserver"
2026-05-23T10:28:50.847285+0100 INFO 	 MX mx1.paypalcorp.com 173.224.165.17
2026-05-23T10:28:50.847830+0100 INFO 	 MX mx2.paypalcorp.com 173.224.161.141
2026-05-23T10:28:51.001912+0100 INFO 	 A paypal.com 151.101.195.1
2026-05-23T10:28:51.002107+0100 INFO 	 A paypal.com 162.159.141.96
2026-05-23T10:28:51.002252+0100 INFO 	 A paypal.com 151.101.3.1
2026-05-23T10:28:51.232181+0100 INFO 	 TXT paypal.com adobe-idp-site-verification=11600efbec96c0e73dd8820cd33ca906ec4302aea4487d208a42a2b01806144c
2026-05-23T10:28:51.232747+0100 INFO 	 TXT paypal.com atlassian-domain-verification=Q8BdHlO6NYSN5njfC2rlbPQxksVfADlcxarxq4fesYJErtGKylvfcfyfwrPD/wnv
2026-05-23T10:28:51.233210+0100 INFO 	 TXT paypal.com v=spf1 include:pp._spf.paypal.com include:3ph1._spf.paypal.com include:3ph2._spf.paypal.com include:3ph3._spf.paypal.com include:3ph4._spf.paypal.com include:sendgrid.net include:aspmx.pardot.com ~all
2026-05-23T10:28:51.233690+0100 INFO 	 TXT paypal.com MS=ms95960309
2026-05-23T10:28:51.234132+0100 INFO 	 TXT paypal.com mgf84gx1cv1c759pmjqx0wnths9ss9f6
2026-05-23T10:28:51.234513+0100 INFO 	 TXT paypal.com docker-verification=2deb3c1f-56d2-4fe4-8a09-d48b7bf8a918
2026-05-23T10:28:51.234875+0100 INFO 	 TXT paypal.com workplace-domain-verification=F7ezsH9uapvYDGd2VtPARy1qq9ymN6
2026-05-23T10:28:51.235273+0100 INFO 	 TXT paypal.com globalsign-domain-verification=KXa3jn_dNODlTVQ4eg1Wx3vA-RrHZ2K7iLQN0vdJBx
2026-05-23T10:28:51.235693+0100 INFO 	 TXT paypal.com mgverify=e00c4bf7480ee22be851faa9acd20e41b8fd0f7b75b434bbe38aa257e5aae3a0
2026-05-23T10:28:51.236145+0100 INFO 	 TXT paypal.com intersight=6d86ec09a7c6926c6f9b8eff8ef0ef06679d84aab4999756a0920a8d430ed8ae
2026-05-23T10:28:51.236270+0100 INFO 	 TXT paypal.com Notion_verify_uVqjH2PpjVthR9xxfR5BZGsuYGtqb6Za4uDHPaA917v5Cg5J0rRwiATz84PWHZh8Px7vFK
2026-05-23T10:28:51.236399+0100 INFO 	 TXT paypal.com stripe-verification=549bef27619f14f935a84c6a23492e80f49ff57a341d9ddc74d8486881cd0d8c
2026-05-23T10:28:51.236521+0100 INFO 	 TXT _dmarc.paypal.com v=DMARC1; p=reject; rua=mailto:d@rua.agari.com; ruf=mailto:d@ruf.agari.com
2026-05-23T10:28:51.305985+0100 INFO 	 TXT _domainkey.paypal.com t=y; o=~;
2026-05-23T10:28:51.306570+0100 INFO Enumerating SRV Records
2026-05-23T10:28:51.483728+0100 INFO 	 SRV _xmpp-server._tcp.paypal.com xmpp.paypal.com 185.97.80.136 5269
2026-05-23T10:28:51.484294+0100 INFO 	 SRV _xmpp-server._tcp.paypal.com xmpp.paypal.com 185.97.80.137 5269
2026-05-23T10:28:51.484690+0100 INFO 	 SRV _xmpp-server._tcp.paypal.com xmpp.paypal.com 173.224.160.141 5269
2026-05-23T10:28:51.485046+0100 INFO 	 SRV _xmpp-server._tcp.paypal.com xmpp.paypal.com 173.224.160.144 5269
2026-05-23T10:28:51.513062+0100 INFO 	 SRV _sipfederationtls._tcp.paypal.com sipfed.online.lync.com 52.112.87.88 5061
2026-05-23T10:28:51.535898+0100 INFO 5 Records Found
2026-05-23T10:28:51.536716+0100 INFO Completed enumeration for domain: paypal.com


## Origin IP Leak 

`for sub in origin direct api internal; do
  dig $sub.paypal.com +short
done
`
api.glb.paypal.com.
173.0.92.23

## Adobe subdomain takeover

`curl -I https://i.paypal.com/ee --resolve i.paypal.com:443:63.140.38.107 
HTTP/2 200
`

x-request-id: 3c67eec8-11f8-4d27-bb43-98f4796f0dc5-735f2e6532e14992
vary: Origin
date: Sat, 23 May 2026 09:50:51 GMT
x-konductor: 26.5.34-HEAD-SNAPSHOT:3d72460e8
x-adobe-edge: VA6;7
server: jag
content-type: text/plain;charset=utf-8
content-length: 40
cache-control: no-cache, no-store, max-age=0, no-transform, private
x-xss-protection: 1; mode=block
x-content-type-options: nosniff
strict-transport-security: max-age=31536000; includeSubDomains


# Nmap Polite 10 scan

`nmap -Pn -p 22,80,443,8080,8443,3000,5000,8000,9000,9090 -vv -sC -sV -sS 173.0.92.23
`

Starting Nmap 7.99 ( https://nmap.org ) at 2026-05-23 11:08 +0100
NSE: Loaded 158 scripts for scanning.
NSE: Script Pre-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 11:08
Completed NSE at 11:08, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 11:08
Completed NSE at 11:08, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 11:08
Completed NSE at 11:08, 0.00s elapsed
Initiating Parallel DNS resolution of 1 host. at 11:08
Completed Parallel DNS resolution of 1 host. at 11:08, 0.50s elapsed
Initiating SYN Stealth Scan at 11:08
Scanning 173.0.92.23 [10 ports]
Discovered open port 8080/tcp on 173.0.92.23
Discovered open port 443/tcp on 173.0.92.23
Discovered open port 80/tcp on 173.0.92.23
Discovered open port 8443/tcp on 173.0.92.23
Completed SYN Stealth Scan at 11:08, 1.64s elapsed (10 total ports)
Initiating Service scan at 11:08
Scanning 4 services on 173.0.92.23
Completed Service scan at 11:08, 12.15s elapsed (4 services on 1 host)
NSE: Script scanning 173.0.92.23.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 11:08
Completed NSE at 11:08, 5.12s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 11:08
Completed NSE at 11:08, 1.64s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 11:08
Completed NSE at 11:08, 0.01s elapsed
Nmap scan report for 173.0.92.23
Host is up, received user-set (0.097s latency).
Scanned at 2026-05-23 11:08:21 WAT for 20s

PORT     STATE    SERVICE    REASON         VERSION
22/tcp   filtered ssh        no-response
80/tcp   open     http       syn-ack ttl 53 Cloudflare http proxy
|_http-title: Site doesn't have a title (text/plain; charset=UTF-8).
|_http-server-header: cloudflare
443/tcp  open     ssl/http   syn-ack ttl 53 Cloudflare http proxy
|_http-server-header: cloudflare
| tls-alpn: 
|   h2
|_  http/1.1
|_http-title: 403 Forbidden
| tls-nextprotoneg: 
|   h2
|_  http/1.1
| ssl-cert: Subject: commonName=api.paypal.com/organizationName=PayPal, Inc./stateOrProvinceName=California/countryName=US/localityName=San Jose
| Subject Alternative Name: DNS:api.paypal.com, DNS:a.paypal.com, DNS:adjvendor.paypal.com, DNS:api-3t.paypal.com, DNS:api-aa-3t.paypal.com, DNS:api-aa.paypal.com, DNS:api-m.paypal.com, DNS:payflowpro.paypal.com, DNS:pilot-payflowpro.paypal.com, DNS:pointofsale-s.paypal.com, DNS:pointofsale.paypal.com, DNS:svcs.paypal.com, DNS:uptycsbrt.paypal.com, DNS:uptycshap.paypal.com, DNS:uptycshon.paypal.com, DNS:uptycsize.paypal.com, DNS:uptycspay.paypal.com, DNS:uptycsven.paypal.com, DNS:zootapi.paypal.com
| Issuer: commonName=DigiCert Global G2 TLS RSA SHA256 2020 CA1/organizationName=DigiCert Inc/countryName=US
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2026-02-02T00:00:00
| Not valid after:  2027-03-05T23:59:59
| MD5:     063d f7fb 9764 e964 21cf ca35 b30f f103
| SHA-1:   30ad ce43 7545 b654 8c1c 2df3 6e49 f26e d420 0519
| SHA-256: 4a10 ca7c 5d2b 13a2 fb60 86b0 19b5 3c33 0176 48f5 d069 0fa3 2fbf f157 d5ab 6a67
| -----BEGIN CERTIFICATE-----
| MIIIUTCCBzmgAwIBAgIQCBwRdBWQ/X+RfjXPf36GHTANBgkqhkiG9w0BAQsFADBZ
| MQswCQYDVQQGEwJVUzEVMBMGA1UEChMMRGlnaUNlcnQgSW5jMTMwMQYDVQQDEypE
| aWdpQ2VydCBHbG9iYWwgRzIgVExTIFJTQSBTSEEyNTYgMjAyMCBDQTEwHhcNMjYw
| MjAyMDAwMDAwWhcNMjcwMzA1MjM1OTU5WjBlMQswCQYDVQQGEwJVUzETMBEGA1UE
| CBMKQ2FsaWZvcm5pYTERMA8GA1UEBxMIU2FuIEpvc2UxFTATBgNVBAoTDFBheVBh
| bCwgSW5jLjEXMBUGA1UEAxMOYXBpLnBheXBhbC5jb20wggEiMA0GCSqGSIb3DQEB
| AQUAA4IBDwAwggEKAoIBAQD8lsDdJQ/Sg5PUCyrS9f5DjoWystWFaovKSrFAz2pW
| IIxfIHiIJRfl6YZE6oJsBbTpS06GLNcjJiAyt2Y5FMZsCOz2Mlp7lVhvidf11lgN
| bKxnRmkWFHA00ljaAGODOMvPj7BYca8vQN9kvTEarsOyh1FGU9xrCfm57D5xrehn
| dk9nCMDEtcEC0NCZOaLM9fKGoka/5PefC/Vti/guAIA0GGth+PL9sTXJNK73K2oi
| EZ7Ui12vFtg4C6iuOLeWksBsh/jdMzXMXwNIgtkZ+vzfZoniVMpgPhCYN4zIRJKk
| vsVz9fTxNkTSGG6vE+VeY24OEAgFJ5lqoX668TTkRbxRAgMBAAGjggUHMIIFAzAf
| BgNVHSMEGDAWgBR0hYDAZsffN97PvSk3qgMdvu3NFzAdBgNVHQ4EFgQUGchooRIB
| 3vmWH4o3l+dBoKg/ofcwggGeBgNVHREEggGVMIIBkYIOYXBpLnBheXBhbC5jb22C
| DGEucGF5cGFsLmNvbYIUYWRqdmVuZG9yLnBheXBhbC5jb22CEWFwaS0zdC5wYXlw
| YWwuY29tghRhcGktYWEtM3QucGF5cGFsLmNvbYIRYXBpLWFhLnBheXBhbC5jb22C
| EGFwaS1tLnBheXBhbC5jb22CFXBheWZsb3dwcm8ucGF5cGFsLmNvbYIbcGlsb3Qt
| cGF5Zmxvd3Byby5wYXlwYWwuY29tghhwb2ludG9mc2FsZS1zLnBheXBhbC5jb22C
| FnBvaW50b2ZzYWxlLnBheXBhbC5jb22CD3N2Y3MucGF5cGFsLmNvbYIUdXB0eWNz
| YnJ0LnBheXBhbC5jb22CFHVwdHljc2hhcC5wYXlwYWwuY29tghR1cHR5Y3Nob24u
| cGF5cGFsLmNvbYIUdXB0eWNzaXplLnBheXBhbC5jb22CFHVwdHljc3BheS5wYXlw
| YWwuY29tghR1cHR5Y3N2ZW4ucGF5cGFsLmNvbYISem9vdGFwaS5wYXlwYWwuY29t
| MD4GA1UdIAQ3MDUwMwYGZ4EMAQICMCkwJwYIKwYBBQUHAgEWG2h0dHA6Ly93d3cu
| ZGlnaWNlcnQuY29tL0NQUzAOBgNVHQ8BAf8EBAMCBaAwEwYDVR0lBAwwCgYIKwYB
| BQUHAwEwgZ8GA1UdHwSBlzCBlDBIoEagRIZCaHR0cDovL2NybDMuZGlnaWNlcnQu
| Y29tL0RpZ2lDZXJ0R2xvYmFsRzJUTFNSU0FTSEEyNTYyMDIwQ0ExLTEuY3JsMEig
| RqBEhkJodHRwOi8vY3JsNC5kaWdpY2VydC5jb20vRGlnaUNlcnRHbG9iYWxHMlRM
| U1JTQVNIQTI1NjIwMjBDQTEtMS5jcmwwgYcGCCsGAQUFBwEBBHsweTAkBggrBgEF
| BQcwAYYYaHR0cDovL29jc3AuZGlnaWNlcnQuY29tMFEGCCsGAQUFBzAChkVodHRw
| Oi8vY2FjZXJ0cy5kaWdpY2VydC5jb20vRGlnaUNlcnRHbG9iYWxHMlRMU1JTQVNI
| QTI1NjIwMjBDQTEtMS5jcnQwDAYDVR0TAQH/BAIwADCCAX4GCisGAQQB1nkCBAIE
| ggFuBIIBagFoAHcATGPcmOWcHauI9h6KPd6uj6tEozd7X5uUw/uhnPzBviYAAAGc
| HZ/7PgAABAMASDBGAiEAqiluw4IfBKeXTp2i/3Q1EhYByZeZqH6RZnH9fNXGIUAC
| IQC6rxAcQpRgfDGmqYO3o5haIoA22ON84384VLEB75hdnAB2AByfaCzp+vBFaVD4
| G5aKh93bMhDYTObIsuOCUkrEz1mfAAABnB2f+0EAAAQDAEcwRQIgUpshdqRYl6iS
| B2lHjYRUxICKiCdea8TVWDZu66vpjlgCIQCEOMIVMaKTyxOYh+Wk45Y25Iy00sBQ
| joGbFt8KGv/n8gB1AGBMmq96f3dfAdQG/JINyJnrCxx9+MlSG/r6F3c7l4vJAAAB
| nB2f/AIAAAQDAEYwRAIgBdarewutFKT1sYvE98+q0aiytqnzymwsjI7SHMl6++IC
| IFAyQcH4Ip6fylCB6TGffklFhzu6F9dWBz+Kq5UZkqdKMA0GCSqGSIb3DQEBCwUA
| A4IBAQAj1IVamRTgHq5XF3r5zSb14OqhG/IRm9K8CuPw2U71WXxmzGbABGCzA5vn
| It213KUkweOb81ONkXNPHITpDuBufRRF0Qd1KOs3Drf+Wtysj65h/eRpnSfHTV3L
| cA7o37sYDuyugiRQIGV83BsIqvy5XW5uc69HdJIcpQx5LLNVaQ1O5Dhqr7P90Cjt
| /nkWj9IsMItD1wYsGKQm3VKTxIpQb0XVJRYYjTuN8id/6OLUmE6NZm+vZczU3REr
| xjbNHGGX1AJmMOoKV0JoCYN23p2xrCUY5f8W3xsAUb0SaRFiYRuIN4nFPCP7MJJv
| dvYUPN1l57MU9JuFiH90GRt5CIa9
|_-----END CERTIFICATE-----
|_ssl-date: TLS randomness does not represent time
3000/tcp filtered ppp        no-response
5000/tcp filtered upnp       no-response
8000/tcp filtered http-alt   no-response
8080/tcp open     http       syn-ack ttl 53 Cloudflare http proxy
|_http-server-header: cloudflare
|_http-title: Site doesn't have a title (text/plain; charset=UTF-8).
8443/tcp open     ssl/http   syn-ack ttl 53 Cloudflare http proxy
|_ssl-date: TLS randomness does not represent time
|_http-title: 403 Forbidden
| tls-alpn: 
|   h2
|_  http/1.1
|_http-server-header: cloudflare
| ssl-cert: Subject: commonName=api.paypal.com/organizationName=PayPal, Inc./stateOrProvinceName=California/countryName=US/localityName=San Jose
| Subject Alternative Name: DNS:api.paypal.com, DNS:a.paypal.com, DNS:adjvendor.paypal.com, DNS:api-3t.paypal.com, DNS:api-aa-3t.paypal.com, DNS:api-aa.paypal.com, DNS:api-m.paypal.com, DNS:payflowpro.paypal.com, DNS:pilot-payflowpro.paypal.com, DNS:pointofsale-s.paypal.com, DNS:pointofsale.paypal.com, DNS:svcs.paypal.com, DNS:uptycsbrt.paypal.com, DNS:uptycshap.paypal.com, DNS:uptycshon.paypal.com, DNS:uptycsize.paypal.com, DNS:uptycspay.paypal.com, DNS:uptycsven.paypal.com, DNS:zootapi.paypal.com
| Issuer: commonName=DigiCert Global G2 TLS RSA SHA256 2020 CA1/organizationName=DigiCert Inc/countryName=US
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2026-02-02T00:00:00
| Not valid after:  2027-03-05T23:59:59
| MD5:     063d f7fb 9764 e964 21cf ca35 b30f f103
| SHA-1:   30ad ce43 7545 b654 8c1c 2df3 6e49 f26e d420 0519
| SHA-256: 4a10 ca7c 5d2b 13a2 fb60 86b0 19b5 3c33 0176 48f5 d069 0fa3 2fbf f157 d5ab 6a67
| -----BEGIN CERTIFICATE-----
| MIIIUTCCBzmgAwIBAgIQCBwRdBWQ/X+RfjXPf36GHTANBgkqhkiG9w0BAQsFADBZ
| MQswCQYDVQQGEwJVUzEVMBMGA1UEChMMRGlnaUNlcnQgSW5jMTMwMQYDVQQDEypE
| aWdpQ2VydCBHbG9iYWwgRzIgVExTIFJTQSBTSEEyNTYgMjAyMCBDQTEwHhcNMjYw
| MjAyMDAwMDAwWhcNMjcwMzA1MjM1OTU5WjBlMQswCQYDVQQGEwJVUzETMBEGA1UE
| CBMKQ2FsaWZvcm5pYTERMA8GA1UEBxMIU2FuIEpvc2UxFTATBgNVBAoTDFBheVBh
| bCwgSW5jLjEXMBUGA1UEAxMOYXBpLnBheXBhbC5jb20wggEiMA0GCSqGSIb3DQEB
| AQUAA4IBDwAwggEKAoIBAQD8lsDdJQ/Sg5PUCyrS9f5DjoWystWFaovKSrFAz2pW
| IIxfIHiIJRfl6YZE6oJsBbTpS06GLNcjJiAyt2Y5FMZsCOz2Mlp7lVhvidf11lgN
| bKxnRmkWFHA00ljaAGODOMvPj7BYca8vQN9kvTEarsOyh1FGU9xrCfm57D5xrehn
| dk9nCMDEtcEC0NCZOaLM9fKGoka/5PefC/Vti/guAIA0GGth+PL9sTXJNK73K2oi
| EZ7Ui12vFtg4C6iuOLeWksBsh/jdMzXMXwNIgtkZ+vzfZoniVMpgPhCYN4zIRJKk
| vsVz9fTxNkTSGG6vE+VeY24OEAgFJ5lqoX668TTkRbxRAgMBAAGjggUHMIIFAzAf
| BgNVHSMEGDAWgBR0hYDAZsffN97PvSk3qgMdvu3NFzAdBgNVHQ4EFgQUGchooRIB
| 3vmWH4o3l+dBoKg/ofcwggGeBgNVHREEggGVMIIBkYIOYXBpLnBheXBhbC5jb22C
| DGEucGF5cGFsLmNvbYIUYWRqdmVuZG9yLnBheXBhbC5jb22CEWFwaS0zdC5wYXlw
| YWwuY29tghRhcGktYWEtM3QucGF5cGFsLmNvbYIRYXBpLWFhLnBheXBhbC5jb22C
| EGFwaS1tLnBheXBhbC5jb22CFXBheWZsb3dwcm8ucGF5cGFsLmNvbYIbcGlsb3Qt
| cGF5Zmxvd3Byby5wYXlwYWwuY29tghhwb2ludG9mc2FsZS1zLnBheXBhbC5jb22C
| FnBvaW50b2ZzYWxlLnBheXBhbC5jb22CD3N2Y3MucGF5cGFsLmNvbYIUdXB0eWNz
| YnJ0LnBheXBhbC5jb22CFHVwdHljc2hhcC5wYXlwYWwuY29tghR1cHR5Y3Nob24u
| cGF5cGFsLmNvbYIUdXB0eWNzaXplLnBheXBhbC5jb22CFHVwdHljc3BheS5wYXlw
| YWwuY29tghR1cHR5Y3N2ZW4ucGF5cGFsLmNvbYISem9vdGFwaS5wYXlwYWwuY29t
| MD4GA1UdIAQ3MDUwMwYGZ4EMAQICMCkwJwYIKwYBBQUHAgEWG2h0dHA6Ly93d3cu
| ZGlnaWNlcnQuY29tL0NQUzAOBgNVHQ8BAf8EBAMCBaAwEwYDVR0lBAwwCgYIKwYB
| BQUHAwEwgZ8GA1UdHwSBlzCBlDBIoEagRIZCaHR0cDovL2NybDMuZGlnaWNlcnQu
| Y29tL0RpZ2lDZXJ0R2xvYmFsRzJUTFNSU0FTSEEyNTYyMDIwQ0ExLTEuY3JsMEig
| RqBEhkJodHRwOi8vY3JsNC5kaWdpY2VydC5jb20vRGlnaUNlcnRHbG9iYWxHMlRM
| U1JTQVNIQTI1NjIwMjBDQTEtMS5jcmwwgYcGCCsGAQUFBwEBBHsweTAkBggrBgEF
| BQcwAYYYaHR0cDovL29jc3AuZGlnaWNlcnQuY29tMFEGCCsGAQUFBzAChkVodHRw
| Oi8vY2FjZXJ0cy5kaWdpY2VydC5jb20vRGlnaUNlcnRHbG9iYWxHMlRMU1JTQVNI
| QTI1NjIwMjBDQTEtMS5jcnQwDAYDVR0TAQH/BAIwADCCAX4GCisGAQQB1nkCBAIE
| ggFuBIIBagFoAHcATGPcmOWcHauI9h6KPd6uj6tEozd7X5uUw/uhnPzBviYAAAGc
| HZ/7PgAABAMASDBGAiEAqiluw4IfBKeXTp2i/3Q1EhYByZeZqH6RZnH9fNXGIUAC
| IQC6rxAcQpRgfDGmqYO3o5haIoA22ON84384VLEB75hdnAB2AByfaCzp+vBFaVD4
| G5aKh93bMhDYTObIsuOCUkrEz1mfAAABnB2f+0EAAAQDAEcwRQIgUpshdqRYl6iS
| B2lHjYRUxICKiCdea8TVWDZu66vpjlgCIQCEOMIVMaKTyxOYh+Wk45Y25Iy00sBQ
| joGbFt8KGv/n8gB1AGBMmq96f3dfAdQG/JINyJnrCxx9+MlSG/r6F3c7l4vJAAAB
| nB2f/AIAAAQDAEYwRAIgBdarewutFKT1sYvE98+q0aiytqnzymwsjI7SHMl6++IC
| IFAyQcH4Ip6fylCB6TGffklFhzu6F9dWBz+Kq5UZkqdKMA0GCSqGSIb3DQEBCwUA
| A4IBAQAj1IVamRTgHq5XF3r5zSb14OqhG/IRm9K8CuPw2U71WXxmzGbABGCzA5vn
| It213KUkweOb81ONkXNPHITpDuBufRRF0Qd1KOs3Drf+Wtysj65h/eRpnSfHTV3L
| cA7o37sYDuyugiRQIGV83BsIqvy5XW5uc69HdJIcpQx5LLNVaQ1O5Dhqr7P90Cjt
| /nkWj9IsMItD1wYsGKQm3VKTxIpQb0XVJRYYjTuN8id/6OLUmE6NZm+vZczU3REr
| xjbNHGGX1AJmMOoKV0JoCYN23p2xrCUY5f8W3xsAUb0SaRFiYRuIN4nFPCP7MJJv
| dvYUPN1l57MU9JuFiH90GRt5CIa9
|_-----END CERTIFICATE-----
| tls-nextprotoneg: 
|   h2
|_  http/1.1
9000/tcp filtered cslistener no-response
9090/tcp filtered zeus-admin no-response

NSE: Script Post-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 11:08
Completed NSE at 11:08, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 11:08
Completed NSE at 11:08, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 11:08
Completed NSE at 11:08, 0.00s elapsed
Read data files from: /usr/share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 21.39 seconds
           Raw packets sent: 17 (748B) | Rcvd: 5 (220B)


# Unusual port 80 open

`curl -v -H "Host: api.paypal.com" http://173.0.92.23/`

*   Trying 173.0.92.23:80...
* Established connection to 173.0.92.23 (173.0.92.23 port 80) from 10.0.0.200 port 46806 
* using HTTP/1.x
> GET / HTTP/1.1
> Host: api.paypal.com
> User-Agent: curl/8.19.0
> Accept: */*
> 
* Request completely sent off
< HTTP/1.1 403 Forbidden
< Date: Sat, 23 May 2026 10:15:07 GMT
< Content-Type: text/html; charset=UTF-8
< Transfer-Encoding: chunked
< Connection: keep-alive
< Cache-Control: private, max-age=0, no-store, no-cache, must-revalidate, post-check=0, pre-check=0
< Expires: Thu, 01 Jan 1970 00:00:01 GMT
< Referrer-Policy: same-origin
< X-Frame-Options: SAMEORIGIN
< set-cookie: __cf_bm=OyJw7fIXtoH6eMLnxEFHOt9gnV387g85VIxNloSLkdc-1779531307.031205-1.0.1.1-CfoDyoz1nMlrP2cNG.Q9yHLL25_UIDfu0ACdKxhLvX.jms9dnp51G7hKAso5vdilTOy96ZUtpUNZDD3jckryy5k2aGK6sKCm6NWG_JKhRfhvSFxhiIuSJqIrQaHEfx8s; HttpOnly; Path=/; Domain=api.paypal.com; Expires=Sat, 23 May 2026 10:45:07 GMT
< Server: cloudflare
< CF-RAY: a0034c2cfaacae14-IAD
< 
<!DOCTYPE html>
<!--[if lt IE 7]> <html class="no-js ie6 oldie" lang="en-US"> <![endif]-->
<!--[if IE 7]>    <html class="no-js ie7 oldie" lang="en-US"> <![endif]-->
<!--[if IE 8]>    <html class="no-js ie8 oldie" lang="en-US"> <![endif]-->
<!--[if gt IE 8]><!--> <html class="no-js" lang="en-US"> <!--<![endif]-->
<head>
<title>Attention Required! | Cloudflare</title>
<meta charset="UTF-8" />
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
<meta http-equiv="X-UA-Compatible" content="IE=Edge" />
<meta name="robots" content="noindex, nofollow" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<link rel="stylesheet" id="cf_styles-css" href="/cdn-cgi/styles/cf.errors.css" />
<!--[if lt IE 9]><link rel="stylesheet" id='cf_styles-ie-css' href="/cdn-cgi/styles/cf.errors.ie.css" /><![endif]-->
<style>body{margin:0;padding:0}</style>


<!--[if gte IE 10]><!-->
<script>
  if (!navigator.cookieEnabled) {
    window.addEventListener('DOMContentLoaded', function () {
      var cookieEl = document.getElementById('cookie-alert');
      cookieEl.style.display = 'block';
    })
  }
</script>
<!--<![endif]-->

</head>
<body>
  <div id="cf-wrapper">
    <div class="cf-alert cf-alert-error cf-cookie-error" id="cookie-alert" data-translate="enable_cookies">Please enable cookies.</div>
    <div id="cf-error-details" class="cf-error-details-wrapper">
      <div class="cf-wrapper cf-header cf-error-overview">
        <h1 data-translate="block_headline">Sorry, you have been blocked</h1>
        <h2 class="cf-subheadline"><span data-translate="unable_to_access">You are unable to access</span> api.paypal.com</h2>
      </div><!-- /.header -->

      <div class="cf-section cf-highlight">
        <div class="cf-wrapper">
          <div class="cf-screenshot-container cf-screenshot-full">
            
              <span class="cf-no-screenshot error"></span>
            
          </div>
        </div>
      </div><!-- /.captcha-container -->

      <div class="cf-section cf-wrapper">
        <div class="cf-columns two">
          <div class="cf-column">
            <h2 data-translate="blocked_why_headline">Why have I been blocked?</h2>

            <p data-translate="blocked_why_detail">This website is using a security service to protect itself from online attacks. The action you just performed triggered the security solution. There are several actions that could trigger this block including submitting a certain word or phrase, a SQL command or malformed data.</p>
          </div>

          <div class="cf-column">
            <h2 data-translate="blocked_resolve_headline">What can I do to resolve this?</h2>

            <p data-translate="blocked_resolve_detail">You can email the site owner to let them know you were blocked. Please include what you were doing when this page came up and the Cloudflare Ray ID found at the bottom of this page.</p>
          </div>
        </div>
      </div><!-- /.section -->

      <div class="cf-error-footer cf-wrapper w-240 lg:w-full py-10 sm:py-4 sm:px-8 mx-auto text-center sm:text-left border-solid border-0 border-t border-gray-300">
    <p class="text-13">
      <span class="cf-footer-item sm:block sm:mb-1">Cloudflare Ray ID: <strong class="font-semibold">a0034c2cfaacae14</strong></span>
      <span class="cf-footer-separator sm:hidden">&bull;</span>
      <span id="cf-footer-item-ip" class="cf-footer-item hidden sm:block sm:mb-1">
        Your IP:
        <button type="button" id="cf-footer-ip-reveal" class="cf-footer-ip-reveal-btn">Click to reveal</button>
        <span class="hidden" id="cf-footer-ip">69.243.67.173</span>
        <span class="cf-footer-separator sm:hidden">&bull;</span>
      </span>
      <span class="cf-footer-item sm:block sm:mb-1"><span>Performance &amp; security by</span> <a rel="noopener noreferrer" href="https://www.cloudflare.com/5xx-error-landing" id="brand_link" target="_blank">Cloudflare</a></span>
      
    </p>
    <script>(function(){function d(){var b=a.getElementById("cf-footer-item-ip"),c=a.getElementById("cf-footer-ip-reveal");b&&"classList"in b&&(b.classList.remove("hidden"),c.addEventListener("click",function(){c.classList.add("hidden");a.getElementById("cf-footer-ip").classList.remove("hidden")}))}var a=document;document.addEventListener&&a.addEventListener("DOMContentLoaded",d)})();</script>
  </div><!-- /.error-footer -->

    </div><!-- /#cf-error-details -->
  </div><!-- /#cf-wrapper -->

  <script>
    window._cf_translation = {};
    
    
  </script>
</body>
* Connection #0 to host 173.0.92.23:80 left intact
</html>  
