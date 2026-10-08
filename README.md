{
  "dns": {
    "servers": [
      {
        "address": "77.88.8.8",
        "domains": [
          "domain:ad.mail.ru",
          "domain:addthis.com",
          "domain:adfox.ru",
          "domain:adfox.yandex.ru",
          "domain:adjust.com",
          "domain:adlabs.ru",
          "domain:adriver.ru",
          "domain:ads.mail.ru",
          "domain:ads.vk.com",
          "domain:ads.yandex.ru",
          "domain:adsafeprotected.com",
          "domain:adservice.google.com",
          "domain:adsmart.ru",
          "domain:adsrvr.org",
          "domain:adsterra.com",
          "domain:adtarget.me",
          "domain:amplitude.com",
          "domain:an.yandex.ru",
          "domain:appmetrica.yandex.ru",
          "domain:appsflyer.com",
          "domain:apptracer.ru",
          "domain:astralab.ru",
          "domain:awaps.yandex.net",
          "domain:betweendigital.com",
          "domain:buzzoola.com",
          "domain:calltouch.ru",
          "domain:chartbeat.com",
          "domain:clarity.ms",
          "domain:connect.facebook.net",
          "domain:counter.rambler.ru",
          "domain:counter.yadro.ru",
          "domain:criteo.com",
          "domain:criteo.net",
          "domain:devtodev.com",
          "domain:digitaltarget.ru",
          "domain:doubleclick.net",
          "domain:doubleverify.com",
          "domain:flocktory.com",
          "domain:flurry.com",
          "domain:getintent.com",
          "domain:gnezdo.ru",
          "domain:google-analytics.com",
          "domain:googleadservices.com",
          "domain:googlesyndication.com",
          "domain:googletagmanager.com",
          "domain:hotjar.com",
          "domain:hotlog.ru",
          "domain:kochava.com",
          "domain:lentainform.com",
          "domain:liveinternet.ru",
          "domain:luckyads.pro",
          "domain:marketgid.com",
          "domain:mc.yandex.com",
          "domain:mc.yandex.ru",
          "domain:mediametrics.ru",
          "domain:mediascope.net",
          "domain:mediasniper.ru",
          "domain:mindbox.ru",
          "domain:mixpanel.com",
          "domain:moatads.com",
          "domain:mytracker.ru",
          "domain:openx.net",
          "domain:otm-r.com",
          "domain:outbrain.com",
          "domain:propellerads.com",
          "domain:pubmatic.com",
          "domain:quantserve.com",
          "domain:r.mradx.net",
          "domain:relap.io",
          "domain:report.appmetrica.yandex.net",
          "domain:retailrocket.net",
          "domain:retailrocket.ru",
          "domain:roistat.com",
          "domain:rubiconproject.com",
          "domain:rutarget.ru",
          "domain:scorecardresearch.com",
          "domain:singular.net",
          "domain:smi2.ru",
          "domain:solocpm.com",
          "domain:soloway.ru",
          "domain:startup.mobile.yandex.net",
          "domain:taboola.com",
          "domain:target.my.com",
          "domain:tenjin.io",
          "domain:tns-counter.ru",
          "domain:top-fwz1.mail.ru",
          "domain:top.mail.ru",
          "domain:top100.rambler.ru",
          "domain:tracker.my.com",
          "domain:uptolike.com",
          "domain:videonow.ru",
          "domain:yandexadexchange.net",
          "domain:yieldmo.com",
          "regexp:\\.(ru|su|moscow|tatar)$",
          "regexp:\\.xn--(p1ai|p1acf|d1acj3b|c1avg|80aswg|80asehdb|80adxhks)$",
          "regexp:^(.+\\.)?(vk|vkontakte|vkplay|vkvideo|userapi|vkuser|vkuseraudio|vkuservideo|vkuserlive|mycdn|mradx|yandex|ya|yastatic|yandexcloud|yandexmetrica|yadi|sberbank|sberdevices|sbermarket|sbermegamarket|sbrf|tinkoff|tbank|alfabank|gazprombank|sovcombank|raiffeisen|yoomoney|qiwi|nspk|mironline|ozon|wildberries|wbbasket|wbstatic|avito|lamoda|lmcdn|megamarket|citilink|mvideo|dns-shop|sportmaster|magnit|perekrestok|pyaterochka|vprok|samokat|kuper|kinopoisk|okko|ivi|dzen|rutube|smotrim|kion|litres|zvuk|boosty|vgtrk|gosuslugi|hh|superjob|cian|domclick|drom|2gis|gismeteo|rambler|pikabu|habr|rustore|beeline|megafon|mts|yota|rzd|aeroflot|pochta|cdnvideo|ngenix|selectel|timeweb|drweb|lesta)\\.[a-z]{2,6}$",
          "regexp:^(.+\\.)?(lenta|rt|tass|vtb|1cfresh|beget)\\.com$",
          "regexp:^(.+\\.)?(vk-cdn|vk-portal)\\.net$",
          "regexp:^(.+\\.)?vk-apps\\.com$",
          "regexp:^(.+\\.)?premier\\.one$",
          "regexp:^(.+\\.)?more\\.tv$",
          "regexp:^(.+\\.)?pobeda\\.aero$",
          "regexp:^(.+\\.)?yandex\\.com\\.tr$"
        ],
        "skipFallback": true
      },
      "https://1.1.1.1/dns-query",
      "https://8.8.8.8/dns-query"
    ],
    "disableCache": false,
    "queryStrategy": "UseIPv4",
    "disableFallback": false
  },
  "log": {
    "loglevel": "warning"
  },
  "policy": {
    "levels": {
      "8": {
        "connIdle": 300,
        "handshake": 4,
        "bufferSize": 512,
        "uplinkOnly": 1,
        "downlinkOnly": 1
      }
    },
    "system": {
      "statsOutboundUplink": true,
      "statsOutboundDownlink": true
    }
  },
  "routing": {
    "rules": [
      {
        "type": "field",
        "inboundTag": [
          "dns-in"
        ],
        "outboundTag": "dns-out"
      },
      {
        "type": "field",
        "domain": [
          "domain:ad.mail.ru",
          "domain:addthis.com",
          "domain:adfox.ru",
          "domain:adfox.yandex.ru",
          "domain:adjust.com",
          "domain:adlabs.ru",
          "domain:adriver.ru",
          "domain:ads.mail.ru",
          "domain:ads.vk.com",
          "domain:ads.yandex.ru",
          "domain:adsafeprotected.com",
          "domain:adservice.google.com",
          "domain:adsmart.ru",
          "domain:adsrvr.org",
          "domain:adsterra.com",
          "domain:adtarget.me",
          "domain:amplitude.com",
          "domain:an.yandex.ru",
          "domain:appmetrica.yandex.ru",
          "domain:appsflyer.com",
          "domain:apptracer.ru",
          "domain:astralab.ru",
          "domain:awaps.yandex.net",
          "domain:betweendigital.com",
          "domain:buzzoola.com",
          "domain:calltouch.ru",
          "domain:chartbeat.com",
          "domain:clarity.ms",
          "domain:connect.facebook.net",
          "domain:counter.rambler.ru",
          "domain:counter.yadro.ru",
          "domain:criteo.com",
          "domain:criteo.net",
          "domain:devtodev.com",
          "domain:digitaltarget.ru",
          "domain:doubleclick.net",
          "domain:doubleverify.com",
          "domain:flocktory.com",
          "domain:flurry.com",
          "domain:getintent.com",
          "domain:gnezdo.ru",
          "domain:google-analytics.com",
          "domain:googleadservices.com",
          "domain:googlesyndication.com",
          "domain:googletagmanager.com",
          "domain:hotjar.com",
          "domain:hotlog.ru",
          "domain:kochava.com",
          "domain:lentainform.com",
          "domain:liveinternet.ru",
          "domain:luckyads.pro",
          "domain:marketgid.com",
          "domain:mc.yandex.com",
          "domain:mc.yandex.ru",
          "domain:mediametrics.ru",
          "domain:mediascope.net",
          "domain:mediasniper.ru",
          "domain:mindbox.ru",
          "domain:mixpanel.com",
          "domain:moatads.com",
          "domain:mytracker.ru",
          "domain:openx.net",
          "domain:otm-r.com",
          "domain:outbrain.com",
          "domain:propellerads.com",
          "domain:pubmatic.com",
          "domain:quantserve.com",
          "domain:r.mradx.net",
          "domain:relap.io",
          "domain:report.appmetrica.yandex.net",
          "domain:retailrocket.net",
          "domain:retailrocket.ru",
          "domain:roistat.com",
          "domain:rubiconproject.com",
          "domain:rutarget.ru",
          "domain:scorecardresearch.com",
          "domain:singular.net",
          "domain:smi2.ru",
          "domain:solocpm.com",
          "domain:soloway.ru",
          "domain:startup.mobile.yandex.net",
          "domain:taboola.com",
          "domain:target.my.com",
          "domain:tenjin.io",
          "domain:tns-counter.ru",
          "domain:top-fwz1.mail.ru",
          "domain:top.mail.ru",
          "domain:top100.rambler.ru",
          "domain:tracker.my.com",
          "domain:uptolike.com",
          "domain:videonow.ru",
          "domain:yandexadexchange.net",
          "domain:yieldmo.com"
        ],
        "outboundTag": "block"
      },
      {
        "type": "field",
        "protocol": [
          "bittorrent"
        ],
        "outboundTag": "direct"
      },
      {
        "ip": [
          "127.0.0.0/8",
          "10.0.0.0/8",
          "172.16.0.0/12",
          "192.168.0.0/16",
          "169.254.0.0/16",
          "100.64.0.0/10",
          "224.0.0.0/4",
          "255.255.255.255/32",
          "::1/128",
          "fc00::/7",
          "fe80::/10"
        ],
        "type": "field",
        "outboundTag": "direct"
      },
      {
        "type": "field",
        "domain": [
          "regexp:\\.(ru|su|moscow|tatar)$",
          "regexp:\\.xn--(p1ai|p1acf|d1acj3b|c1avg|80aswg|80asehdb|80adxhks)$",
          "regexp:^(.+\\.)?(vk|vkontakte|vkplay|vkvideo|userapi|vkuser|vkuseraudio|vkuservideo|vkuserlive|mycdn|mradx|yandex|ya|yastatic|yandexcloud|yandexmetrica|yadi|sberbank|sberdevices|sbermarket|sbermegamarket|sbrf|tinkoff|tbank|alfabank|gazprombank|sovcombank|raiffeisen|yoomoney|qiwi|nspk|mironline|ozon|wildberries|wbbasket|wbstatic|avito|lamoda|lmcdn|megamarket|citilink|mvideo|dns-shop|sportmaster|magnit|perekrestok|pyaterochka|vprok|samokat|kuper|kinopoisk|okko|ivi|dzen|rutube|smotrim|kion|litres|zvuk|boosty|vgtrk|gosuslugi|hh|superjob|cian|domclick|drom|2gis|gismeteo|rambler|pikabu|habr|rustore|beeline|megafon|mts|yota|rzd|aeroflot|pochta|cdnvideo|ngenix|selectel|timeweb|drweb|lesta)\\.[a-z]{2,6}$",
          "regexp:^(.+\\.)?(lenta|rt|tass|vtb|1cfresh|beget)\\.com$",
          "regexp:^(.+\\.)?(vk-cdn|vk-portal)\\.net$",
          "regexp:^(.+\\.)?vk-apps\\.com$",
          "regexp:^(.+\\.)?premier\\.one$",
          "regexp:^(.+\\.)?more\\.tv$",
          "regexp:^(.+\\.)?pobeda\\.aero$",
          "regexp:^(.+\\.)?yandex\\.com\\.tr$"
        ],
        "outboundTag": "direct"
      },
      {
        "port": "0-65535",
        "type": "field",
        "outboundTag": "proxy"
      }
    ],
    "domainMatcher": "hybrid",
    "domainStrategy": "AsIs"
  },
  "inbounds": [
    {
      "tag": "socks",
      "port": 10808,
      "listen": "127.0.0.1",
      "protocol": "socks",
      "settings": {
        "udp": true,
        "auth": "noauth",
        "userLevel": 8
      },
      "sniffing": {
        "enabled": true,
        "routeOnly": false,
        "destOverride": [
          "http",
          "tls"
        ]
      }
    },
    {
      "tag": "http",
      "port": 10809,
      "listen": "127.0.0.1",
      "protocol": "http",
      "settings": {
        "userLevel": 8
      }
    },
    {
      "tag": "dns-in",
      "port": 10853,
      "listen": "127.0.0.1",
      "protocol": "dokodemo-door",
      "settings": {
        "port": 53,
        "address": "77.88.8.8",
        "network": "tcp,udp"
      }
    }
  ],
  "outbounds": [
    {
      "tag": "proxy",
      "protocol": "vless",
      "settings": {
        "vnext": [
          {
            "address": "de.bolvankamax.com",
            "port": 443,
            "users": [
              {
                "id": "f2f9b2db-b1c1-4b6f-80b5-99787e0a2141",
                "encryption": "none",
                "flow": ""
              }
            ]
          }
        ]
      },
      "streamSettings": {
        "network": "xhttp",
        "xhttpSettings": {
          "mode": "auto",
          "host": "",
          "path": "/55f318edd8b4"
        },
        "security": "reality",
        "realitySettings": {
          "serverName": "www.zalando.de",
          "publicKey": "l5_EHPg0T4EvagTn883oushyUwVU_GGHDsZr7hHEfXg",
          "shortId": "a41b4f92d7bf092d",
          "fingerprint": "safari"
        }
      }
    },
    {
      "tag": "direct",
      "protocol": "freedom"
    },
    {
      "tag": "block",
      "protocol": "blackhole"
    },
    {
      "tag": "dns-out",
      "protocol": "dns"
    }
  ],
  "remarks": "🇩🇪 Германия"
}
