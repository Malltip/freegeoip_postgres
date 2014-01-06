Freegeoip Update.py for Postgres
================================

[Freegeoip](https://freegeoip.net/) is a great public REST API for searching
geolocation of IP addresses and hostnames. Not only is it free, it is also
open source, available [here](https://github.com/fiorix/freegeoip).

While it is convenient to rely on 3rd party services, it sometimes makes sense to
host it yourself (freegeoip gets DDOSed, you want to reduce network calls, etc). This port
allows you download and insert geo-data into your Postgres Database.

Just change update the connstr variable in updatedb.py (line 26) and you're all set!

    connstr = "CHANGE_ME_TO_YOUR_POSTGRES_CONN_STR"

Thanks to [Alexandre Fiori](https://github.com/fiorix) for creating such an awesome
service.
