[Rewrite]
http-response-jq ^https:\/\/so\.xiaohongshu\.com\/api\/sns\/v\d+\/search\/notes '.data.items |= map(select(.note?.type == "normal"))'
http-response-jq ^https:\/\/rec\.xiaohongshu\.com\/api\/sns\/v\d+\/homefeed '.data |= map(select(.type == "normal"))'


[MITM]
hostname = *.xiaohongshu.com