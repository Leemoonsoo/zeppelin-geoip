zeppelin-geoip
==============


This [Zeppelin](http://zeppelin-project.org) library which adds GeoIP conversion UDF with dependencies and creates a temporary function to use it.




Usage
-------------------

Install 'geoip' through ZAN menu on [Zeppelin](http://zeppelin-project.org)
```
SELECT
  geocode_ip(remote_ip, 'city', 'GeoLiteCity.dat') as city,
  geocode_ip(remote_ip, 'country', 'GeoLiteCity.dat') as country
FROM nginx_log limit 50;
```

Source
-------------------
[Hive UDF](https://github.com/sharethrough/hive-udfs) 


