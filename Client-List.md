## What are Client Lists?
- Client Lists are a replacement for the existing Network Lists. With Client Lists, you can create new types of lists, use multiple criteria for filtering the incoming web traffic, track saved changes more easily, and also search, sort, modify, and activate lists. It allows you to filter web requests not only by IP and Geo location, but an additional number of parameters, and offers wider functionality, as well as even more intuitive change tracking, list modification, and list activation.
- Client Lists are collections of web request characteristics, based on which you can block or allow client access. There are numerous types of lists you can create, depending on what kind of client request characteristics you would like to group together, and fine-tune which incoming requests you want to accept.

## What are types of Client Lists we can create?
- **IP/CIDR** - containing IPv4 or IPv6 addresses;
- **Geo location** - which contain countries from where requests originate;
- **ASN** - containing Autonomous System numbers with a decimal value between 0 and 4294967295;
- **File hash** - containing SHA-256 file hashes,
- **TLS fingerprint** - containing a representation of data exchanged during a TLS handshake.

## What are the limitations of Client Lists?
- The limit of lists you can create per account is 1000
- The limit of lists you can reference in a single configuration is up to 100 with Client Lists, as opposed to a maximum of 32 with Network Lists.
- Depending on the type of list you're creating, there's a limit of entries you can add
  - for an IP list, up to 10 000 entries
  - for a geo list, up to 275 entries
  - for a TLS fingerprint list, up to 100 entries
  - for an ASN list, up to 100 entries
  - for a file hash list, up to 100 entries

## Why do we have to choose the Client List over Network List?
  
| Network List                       |  Client List                         |
|------------------------------------|:------------------------------------:|
| Supports only IPs/CIDRs, Geo locations | Supports Autonomous System Numbers (ASNs), TLS fingerprints, File hashes, IPs/CIDRs and Geo locations |
| Use up to 32 Network Lists in each security configuration |  Use up to 100 Client Lists in each security configuration |
| Entries doesnt have the tags |    Entries are now configurable with descriptions and tags, as well as added/modified & expiration dates |
| No Bulk operations | Create lists conveniently using bulk paste or CSV upload. Bulk select and modify lists entries at scale |
| Doesnt show the out of sync details between prod / staging | shows the out of sync details between prod / staging |

- Tags help you search and filter lists and their entries. You can add up to five tags at a list as well as entry level, up to 255 characters each
- For each entry you add to your Client List, you can set an expiration date. Once the timer passes the expiration date on an entry, it will still be stored as an expired entry. After 30 days from that point, it will be deleted
- 

