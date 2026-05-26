### whois 173.0.92.23

target = 173.0.92.23

## Passive Scans

`whois $target`

#
# ARIN WHOIS data and services are subject to the Terms of Use
# available at: https://www.arin.net/resources/registry/whois/tou/
#
# If you see inaccuracies in the results, please report at
# https://www.arin.net/resources/registry/whois/inaccuracy_reporting/
#
# Copyright 1997-2026, American Registry for Internet Numbers, Ltd.
#


NetRange:       173.0.80.0 - 173.0.95.255
CIDR:           173.0.80.0/20
NetName:        PAYPAL-SITE
NetHandle:      NET-173-0-80-0-1
Parent:         NET173 (NET-173-0-0-0-0)
NetType:        Direct Allocation
OriginAS:       
Organization:   PayPal, Inc. (PAYPAL)
RegDate:        2010-06-22
Updated:        2021-12-14
Ref:            https://rdap.arin.net/registry/ip/173.0.80.0


OrgName:        PayPal, Inc.
OrgId:          PAYPAL
Address:        2211 N. First St.
City:           San Jose
StateProv:      CA
PostalCode:     95131
Country:        US
RegDate:        2001-08-17
Updated:        2019-04-10
Ref:            https://rdap.arin.net/registry/entity/PAYPAL


OrgAbuseHandle: NETWO8902-ARIN
OrgAbuseName:   Network Abuse
OrgAbusePhone:  +1-480-967-5100 
OrgAbuseEmail:  abuse@paypal.com
OrgAbuseRef:    https://rdap.arin.net/registry/entity/NETWO8902-ARIN

OrgTechHandle: PAYPA-ARIN
OrgTechName:   PayPal Network
OrgTechPhone:  +1-408-967-5100 
OrgTechEmail:  routing@paypal.com
OrgTechRef:    https://rdap.arin.net/registry/entity/PAYPA-ARIN

RAbuseHandle: NETWO8902-ARIN
RAbuseName:   Network Abuse
RAbusePhone:  +1-480-967-5100 
RAbuseEmail:  abuse@paypal.com
RAbuseRef:    https://rdap.arin.net/registry/entity/NETWO8902-ARIN

RNOCHandle: PAYPA1-ARIN
RNOCName:   PayPal
RNOCPhone:  +1-480-967-5100 
RNOCEmail:  routing@paypal.com
RNOCRef:    https://rdap.arin.net/registry/entity/PAYPA1-ARIN

RTechHandle: PAYPA1-ARIN
RTechName:   PayPal
RTechPhone:  +1-480-967-5100 
RTechEmail:  routing@paypal.com
RTechRef:    https://rdap.arin.net/registry/entity/PAYPA1-ARIN


#
# ARIN WHOIS data and services are subject to the Terms of Use
# available at: https://www.arin.net/resources/registry/whois/tou/
#
# If you see inaccuracies in the results, please report at
# https://www.arin.net/resources/registry/whois/inaccuracy_reporting/
#
# Copyright 1997-2026, American Registry for Internet Numbers, Ltd.
#

## DIG

`dig $target`

; <<>> DiG 9.20.22-1-Debian <<>> 173.0.92.23
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NXDOMAIN, id: 54045
;; flags: qr rd ra ad; QUERY: 1, ANSWER: 0, AUTHORITY: 1, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 512
;; QUESTION SECTION:
;173.0.92.23.			IN	A

;; AUTHORITY SECTION:
.			10800	IN	SOA	a.root-servers.net. nstld.verisign-grs.com. 2026052300 1800 900 604800 86400

;; Query time: 1323 msec
;; SERVER: 75.75.75.75#53(75.75.75.75) (UDP)
;; WHEN: Sat May 23 11:25:19 WAT 2026
;; MSG SIZE  rcvd: 115


## Testing each SAN subdomains

`for sub in a adjvendor api-3t api-aa-3t api-aa api-m payflowpro pilot-payflowpro pointofsale-s pointofsale svcs uptycsbrt uptycshap uptycshon uptycsize uptycspay uptycsven zootapi; do
  echo "=== $sub.paypal.com ==="
  curl -k -s -o /dev/null -w "%{http_code}\n" -H "Host: $sub.paypal.com" https://173.0.92.23/
done
`
=== a.paypal.com ===
403
=== adjvendor.paypal.com ===
503
=== api-3t.paypal.com ===
403
=== api-aa-3t.paypal.com ===
403
=== api-aa.paypal.com ===
403
=== api-m.paypal.com ===
403
=== payflowpro.paypal.com ===
403
=== pilot-payflowpro.paypal.com ===
403
=== pointofsale-s.paypal.com ===
404
=== pointofsale.paypal.com ===
403
=== svcs.paypal.com ===
403
=== uptycsbrt.paypal.com ===
403
=== uptycshap.paypal.com ===
403
=== uptycshon.paypal.com ===
403
=== uptycsize.paypal.com ===
403
=== uptycspay.paypal.com ===
403
=== uptycsven.paypal.com ===
403
=== zootapi.paypal.com ===
403
    

## Origin IP exposed headers

`curl -k -H "Host: api.paypal.com" https://173.0.92.23/ -I | grep -E "(x-origin|backend|real-ip|cf-ray)"`

  % Total    % Received % Xferd  Average Speed  Time    Time    Time   Current
                                 Dload  Upload  Total   Spent   Left   Speed
  0   1364   0      0   0      0      0      0                              0
cf-ray: a00361f9eba890ac-IAD
