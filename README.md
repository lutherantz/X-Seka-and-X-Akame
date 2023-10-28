# X-Seka and X-Akame Headers

Hello ! I tried to make 2 Headers, 1 for cookies and params (X-Seka), 2 for data.

## Results

### v1

```python
signer = Signature(
).get_encrypt()
---------------------
> py test.py
X-Seka  : 0!{gw&xXT*ISX.4369348961.J

X-Akame :
```

### v2

```python
signer = Signature(
    cookies = "sessionid=0e957bcf5b70S0S0S0Sa1741571e8dd0210",
).get_encrypt()
---------------------
> py test.py
X-Seka  : 0zyCo(xX'l0r3.0679348961.JwEjMwQGZ4UWM3UTM0cTMhNFMTBzUwMFM3IWNmNmY3UTOlBTPklmbvl2czV2c

X-Akame :
```

### v3

```python
signer = Signature(
    data = {
        "room_id": 8983738292,
    }
).get_encrypt()
---------------------
> py test.py
X-Seka  : 0.#OB3xXphYKv.8699348961.J

X-Akame : {'==AZp9Vbv9mc': 'I5{{oH#0agIWh'}
```

### v4

```python
params = urlencode({
    "WebIdLastTime": "1697982664",
    "aid": "1988",
    "app_language": "fr",
    "app_name": "tiktok_web",
    "browser_language": "fr-FR",
    "browser_name": "Mozilla",
    "browser_online": True,
    "browser_platform": "Win32",
    "browser_version": "5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Safari/537.36",
    "channel": "tiktok_web",
    "cookie_enabled": True,
    "device_id": "7292779548043134496",
    "device_platform": "web_pc",
    "device_type": "web_h265",
    "focus_state": True,
    "from_page": "user",
    "history_len": 4,
    "is_fullscreen": False,
    "is_page_visible": True,
    "os": "windows",
    "priority_region": "FR",
    "referer": "https://www.tiktok.com/@MS4wLjABAAAAOe_LwpP7P8USPPTX8m0ITMxWA2LOEb2XshqvjB0HnrDa7dZmTwtJj6UYGJnVJxB4",
    "region": "FR",
    "root_referer": "https://www.tiktok.com/@MS4wLjABAAAAOe_LwpP7P8USPPTX8m0ITMxWA2LOEb2XshqvjB0HnrDa7dZmTwtJj6UYGJnVJxB4",
    "screen_height": 1080,
    "screen_width": 1920,
    "tz_name": "Europe/Paris",
    "webcast_language": "fr",
})

signer = Signature(
    params = params
).get_encrypt()
---------------------
> py test.py
X-Seka  : 0c4X3WxXzW!J^^xzb^I-+Y}jLRV@K%VcWop%ag8cDGLNX*ZLh<wJ@XeeZVmkUCY0!*FfgQOW4qMeZ>C&{V2x~4IJUiUb<(coW+<}oW4LO7bLKStc4wV^Ni?RdH>cUXch-jLW_Stzaf{GNLGINmXB5rlVJf7EG9#X?Oxk@7Zrkh*Pn?{8I;fN8apBWnWJ)w|KlF%CY>x5#QiQV{BB{z6ZNA6cYE+`=XyvuXcL{D{BqOx_KyR0Cav`o!J5VZpW;zgvUR>K&a{R{wJ4P8KXoLw$G6qV!R48~wS$M_@N3!%BZ2!-KVOd#NN}T|4c`DWaSf!oePNpx3SEaNmNkD7US;P3&QLf8&Hlc}mO06H~K6@0PLQ$8Tc5fliFdmaDGGId{Ve`=ZbY*7_E266tMbmaDGK-M{BYfZabe`XpW^hBoWnn7pMl>V>X<zgvUVsp%aHv^BahMC+Z9{GWc+{0UC?A0CRSq*rVI2>4cuD|PV2t(>XME$;Y}dqaZ>C&{VN>=!b@s(>X6+paZ0X%0dVT89bLecwas+}#J<X9Aa4*K&aI@8!bK1$jWJ;79b1<8|Vn_~6HmHZuUdeG$JP-`abyz7=XHx+SC$7bqVo8R9ZId^Yb;+OvU}c=4cc|QYHg_+cGUn=fFms;WIljjWIB=ZIWy1X`V~_yMWU`=&a6{?nW<0eeZ!tP=X3Pd{VGK%Vc4{=ZbnY=#J43<fZ}zzSCa?d!HsBbDGD6CRV+=p^DI@)-ET(q*Fa`D{BA*K&aGe(VIoh}iYxES@D{vw-YR-D{BsQ{KNmcD{BOYB;Ex}~lMrt=>XL;l7S8syBaj<3CG8X4scR=M{B&+K>X@pReG94KfF~!;EPmMC+Z!l~7SG{v<Dc;AvJGm^7b31_vUOTMXcL1rSCzzK>XV|0&a1AURV4(j$aLNC+ZB>PhWaddyJ~&w-Y5$j$aLNC+Z7d2JVIHDTdA%#jW-P6vUOTMXcL1rSCu$FxaRKtJX29AfZ=sj$aLNC+Z8mTkV|OQhYE+`=Xl=lDZ=g?9aLJcwaRKtJX29AfZ;a?9am6{3Ir{xuJ0rhSCe3!BGt{5XIA%!jW=|~Wbma3KWJ;l7S74Baf.2100448961.J

X-Akame :
```

### v4

```python
params = urlencode({
    "WebIdLastTime": "1697982664",
    "aid": "1988",
    "app_language": "fr",
    "app_name": "tiktok_web",
    "browser_language": "fr-FR",
    "browser_name": "Mozilla",
    "browser_online": True,
    "browser_platform": "Win32",
    "browser_version": "5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Safari/537.36",
    "channel": "tiktok_web",
    "cookie_enabled": True,
    "device_id": "7292779548043134496",
    "device_platform": "web_pc",
    "device_type": "web_h265",
    "focus_state": True,
    "from_page": "user",
    "history_len": 4,
    "is_fullscreen": False,
    "is_page_visible": True,
    "os": "windows",
    "priority_region": "FR",
    "referer": "https://www.tiktok.com/@MS4wLjABAAAAOe_LwpP7P8USPPTX8m0ITMxWA2LOEb2XshqvjB0HnrDa7dZmTwtJj6UYGJnVJxB4",
    "region": "FR",
    "root_referer": "https://www.tiktok.com/@MS4wLjABAAAAOe_LwpP7P8USPPTX8m0ITMxWA2LOEb2XshqvjB0HnrDa7dZmTwtJj6UYGJnVJxB4",
    "screen_height": 1080,
    "screen_width": 1920,
    "tz_name": "Europe/Paris",
    "webcast_language": "fr",
})

signer = Signature(
    params = params,
    data = {
        "room_id": 8387728828981272263
    },
    cookies = "sessionid=sndnnsn3883Sb8383Nsn"
).get_encrypt()
---------------------
> py test.py
X-Seka  : 0RKz$FxXzW!J^^xzb^I-+Y}jLRV@K%VcWop%ag8cDGLNX*ZLh<wJ@XeeZVmkUCY0!*FfgQOW4qMeZ>C&{V2x~4IJUiUb<(coW+<}oW4LO7bLKStc4wV^Ni?RdH>cUXch-jLW_Stzaf{GNLGINmXB5rlVJf7EG9#X?Oxk@7Zrkh*Pn?{8I;fN8apBWnWJ)w|KlF%CY>x5#QiQV{BB{z6ZNA6cYE+`=XyvuXcL{D{BqOx_KyR0Cav`o!J5VZpW;zgvUR>K&a{R{wJ4P8KXoLw$G6qV!R48~wS$M_@N3!%BZ2!-KVOd#NN}T|4c`DWaSf!oePNpx3SEaNmNkD7US;P3&QLf8&Hlc}mO06H~K6@0PLQ$8Tc5fliFdmaDGGId{Ve`=ZbY*7_E266tMbmaDGK-M{BYfZabe`XpW^hBoWnn7pMl>V>X<zgvUVsp%aHv^BahMC+Z9{GWc+{0UC?A0CRSq*rVI2>4cuD|PV2t(>XME$;Y}dqaZ>C&{VN>=!b@s(>X6+paZ0X%0dVT89bLecwas+}#J<X9Aa4*K&aI@8!bK1$jWJ;79b1<8|Vn_~6HmHZuUdeG$JP-`abyz7=XHx+SC$7bqVo8R9ZId^Yb;+OvU}c=4cc|QYHg_+cGUn=fFms;WIljjWIB=ZIWy1X`V~_yMWU`=&a6{?nW<0eeZ!tP=X3Pd{VGK%Vc4{=ZbnY=#J43<fZ}zzSCa?d!HsBbDGD6CRV+=p^DI@)-ET(q*Fa`D{BA*K&aGe(VIoh}iYxES@D{vw-YR-D{BsQ{KNmcD{BOYB;Ex}~lMrt=>XL;l7S8syBaj<3CG8X4scR=M{B&+K>X@pReG94KfF~!;EPmMC+Z!l~7SG{v<Dc;AvJGm^7b31_vUOTMXcL1rSCzzK>XV|0&a1AURV4(j$aLNC+ZB>PhWaddyJ~&w-Y5$j$aLNC+Z7d2JVIHDTdA%#jW-P6vUOTMXcL1rSCu$FxaRKtJX29AfZ=sj$aLNC+Z8mTkV|OQhYE+`=Xl=lDZ=g?9aLJcwaRKtJX29AfZ;a?9am6{3Ir{xuJ0rhSCe3!BGt{5XIA%!jW=|~Wbma3KWJ;l7S18Cja.0800448961.JuNnTzgzM4I2UzgDOz42cu5GZuNXPklmbvl2czV2c

X-Akame : {'==AZp9Vbv9mc': 'I5RjmH!?UlGB`OnF)}wYGBz^'}
```

### v5

```python
from sign.XSeka import Signature
from pytermx import Color
from urllib.parse import urlencode

signer = Signature(
    cookies = "seka=seka",
    params = "Webid=8928",
    data = {
        "peter": "miles"
    }
).get_encrypt()

print(f"{Color.BRIGHT_YELLOW}X-Seka  {Color.GREY}: {Color.BRIGHT_BLUE}{signer['X-Seka']}\n\n{Color.BRIGHT_YELLOW}X-Akame {Color.GREY}: {Color.BRIGHT_BLUE}{signer['X-Akame']}{Color.RESET}")

print('\n')

signer = Signature().decrypt(
    XSeka = signer['X-Seka'],
    XAkame = signer['X-Akame']
)

print(f"{Color.BRIGHT_YELLOW}X-Seka  {Color.GREY}: {Color.BRIGHT_BLUE}{signer['X-Seka']}\n\n{Color.BRIGHT_YELLOW}X-Akame {Color.GREY}: {Color.BRIGHT_BLUE}{signer['X-Akame']}{Color.RESET}")
---------------------
> py test.py
X-Seka  : 0C35a|xX^BGJ@ZIWp;l7Sa9DP=AKESS.4707948961.JhtWZz1TYrV2cEND_SEKA

X-Akame : {'=IXZ0VGc': 'ZE0*}a{'}


X-Seka  : Cookies=seka=seka;Time=14:44:34;Params=Webid=8928

X-Akame : {'peter': 'miles'}
```
