# PyWhoisAPI
Python wrapper for ARIN WhoisRWS API

PyWhoisAPI is a library for Python that wraps the ARIN WhoisRWS API. Currently, works with Ptyhon 2. This is a fairly old project imported from: https://code.google.com/archive/p/pywhoisapi/. The project is not actively maintained.

More information on WhoisRWS API can be found on: https://www.arin.net/resources/whoisrws/whois_api.html

Questions, comments? rambasnet@gmail.com

Example usage:

```python
import PyWhoisAPI as PW
whois = PW.Whois() print whois.getPointOfContact('KOSTE-ARIN', format='json')
print whois.getPointOfContactsAssociatedWith('org', 'ARIN', 'xml')
print whois.getNetworksAssociatedWith('poc', 'KOSTE-ARIN', 'xml')
print print whois.getUnrelatedListOfOrgs(name='ARIN**')**
print whois.getNetworkRegistrationRelatedToIP('192.149.252.75', format='json')
```
