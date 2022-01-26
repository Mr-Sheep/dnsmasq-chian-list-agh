automatically parsing the latest dnsmasq-china-list from [felixonmars/dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list) for AdGuradHome.

The 114.114.114.114 dns server was replaced by tencent's dns pub DoH server to avoid dns cache poisoning by local isps.

The accelerated-domains.china.default.conf has default dns servers included. We are currently using DNS services provided by Tsinghua University. (since most of the DoH services are blocked by the GFW.) You can surely use Cloudflare Worker to reverse proxy cloudflare's, or some other providers', DNS server.
