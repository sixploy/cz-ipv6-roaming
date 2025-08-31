# České mobilní sítě a IPv6 v roamingu

Tento repozitář si klade za cíl sesbírat poznatky o schopnosti českých mobilních operátorů nabídnout IPv6 během roamingu, tedy při využívání datových služeb pomocí české SIM karty v zahraničí.

## Aktivace IPv6 v roamingu

[Vodafone CZ](https://www.vodafone.cz/) a [T-Mobile CZ](https://www.t-mobile.cz/osobni) mají ve výchozím stavu v roamingu povolen pouze protokol IPv4. IPv6 v roamingu ovšem neblokují, proto si ji můžete aktivně zapnout (viz návod níže).

[O2 CZ](https://www.o2.cz/) v roamingu aktivně blokuje - i pokud si IPv6 v mobilu povolíte, v roamingu vám síť vždy přidělí pouze IPv4 adresu. Proto IPv6 v seznamech níže nenajdete, a **dokud O2 IPv6 v roamingu nezpřístupní, nemá smysl posílat pull requesty se všemi záznamy typu "IPv6 u O2 v této zemi nefunguje"**.

### Aktivace na Androidu

Postupujte například podle [návodu pro Samsung na stránkách T-Mobilu](https://www.t-mobile.cz/dcpublic/TMCZ-Nastaveni_APN_pro_IPv6_Samsung_Galaxy_S20_Ultra_5G.pdf), ale volbu "Protokol přístupového bodu při roamingu" nastavte na `IPv4/IPv6`.

### Aktivace na iOSu

Použijte konfigurátor APN profilů na [fe80.cz](https://fe80.cz/).

## Seznam zemí a sítí

Tento seznam není úplný - zahrnuje pouze kombinace sítí a operátorů, ve kterých jsme české IPv6 aktivně otestovali. Pokud nějaká kombinace v seznamu chybí, prosím, pošlete pull request s doplněním, zda v ní IPv6 funguje, nefunguje, případně zda se do sítě vůbec nelze přihlásit.

### Bulharsko (MCC 284)

| Operátor    | Síť                 | Stav IPv6             |
|-------------|---------------------|-----------------------|
| T-Mobile CZ | Yettel (284 05)     | ✅ Funkční            |
| T-Mobile CZ | Vivacom (284 03)    | ✅ Funkční            |
| T-Mobile CZ | A1/Mobitel (284 01) | ✅ Funkční            |
| Vodafone CZ | Yettel (284 05)     | ✅ Funkční            |
| Vodafone CZ | Vivacom (284 03)    | ⛔️ Nelze se přihlásit |
| Vodafone CZ | A1/Mobitel (284 01) | ✅ Funkční            |

### Dánsko (MCC 238)

| Operátor    | Síť                   | Stav IPv6  |
|-------------|-----------------------|------------|
| T-Mobile CZ | Nuuday/TDC (238 01)   | ✅ Funkční |
| T-Mobile CZ | Telenor (238 02)      | ✅ Funkční |
| T-Mobile CZ | 3 (238 06)            | ✅ Funkční |
| T-Mobile CZ | Telia/Norlys (238 20) | ✅ Funkční |
| Vodafone CZ | Nuuday/TDC (238 01)   | ✅ Funkční |
| Vodafone CZ | Telenor (238 02)      | ✅ Funkční |
| Vodafone CZ | 3 (238 06)            | ✅ Funkční |
| Vodafone CZ | Telia/Norlys (238 20) | ✅ Funkční |

### Francie (MCC 208)

| Operátor    | Síť                       | Stav IPv6  |
|-------------|---------------------------|------------|
| T-Mobile CZ | Orange (208 01)           | ✅ Funkční |
| T-Mobile CZ | SFR (208 10)              | ✅ Funkční |
| T-Mobile CZ | Free (208 15)             | ✅ Funkční |
| T-Mobile CZ | Bouygues Telecom (208 20) | ✅ Funkční |

### Chorvatsko (MCC 219)

| Operátor    | Síť                       | Stav IPv6   |
|-------------|---------------------------|-------------|
| T-Mobile CZ | Hrvatski Telekom (219 01) | ✅ Funkční  |

### Itálie (MCC 222)

| Operátor    | Síť                  | Stav IPv6                                 |
|-------------|----------------------|-------------------------------------------|
| T-Mobile CZ | TIM (222 01)         | 🟧 Funkční v LTE/5G, IPv4-only v GSM/UMTS |
| T-Mobile CZ | Vodafone (222 10)    | ⛔️ Nelze se přihlásit                     |
| T-Mobile CZ | Iliad (222 50)       | ✅ Funkční v LTE i UMTS                   |
| T-Mobile CZ | Wind Tre (222 88/99) | ❌ IPv4-only (v LTE, UMTS, GSM)           |

### Maďarsko (MCC 216)

| Operátor    | Síť                       | Stav IPv6   |
|-------------|---------------------------|-------------|
| T-Mobile CZ | Telekom (216 30)          | ✅ Funkční  |

### Německo (MCC 262)

| Operátor    | Síť                  | Stav IPv6             |
|-------------|----------------------|-----------------------|
| Vodafone CZ | Vodafone DE (260 02) | ✅ Funkční            |
| T-Mobile CZ | Telekom DE (260 01)  | ✅ Funkční            |
| T-Mobile CZ | Vodafone DE (260 02) | ⛔️ Nelze se přihlásit |
| T-Mobile CZ | O2 DE (260 03)       | ✅ Funkční            |

### Polsko (MCC 260)

| Operátor    | Síť               | Stav IPv6  |
|-------------|-------------------|------------|
| T-Mobile CZ | T-Mobile (260 02) | ✅ Funkční |
| T-Mobile CZ | Orange (260 03)   | ✅ Funkční |

### Rakousko (MCC 232)

| Operátor    | Síť                       | Stav IPv6  |
|-------------|---------------------------|------------|
| T-Mobile CZ | Magenta Telekom (232 03)  | ✅ Funkční |

### Slovensko (MCC 231)

| Operátor    | Síť                       | Stav IPv6  |
|-------------|---------------------------|------------|
| T-Mobile CZ | Telekom (231 02)          | ✅ Funkční |

### Slovinsko (MCC 293)

| Operátor    | Síť                       | Stav IPv6  |
|-------------|---------------------------|------------|
| T-Mobile CZ | Telemach (293 70)         | ✅ Funkční |

### Švédsko (MCC 240)

| Operátor    | Síť              | Stav IPv6  |
|-------------|------------------|------------|
| T-Mobile CZ | Telia (240 01)   | ✅ Funkční |
| T-Mobile CZ | 3 (240 02)       | ✅ Funkční |
| T-Mobile CZ | Tele2 (240 07)   | ✅ Funkční |
| T-Mobile CZ | Telenor (240 08) | ✅ Funkční |
| Vodafone CZ | Telia (240 01)   | ✅ Funkční |
| Vodafone CZ | 3 (240 02)       | ✅ Funkční |
| Vodafone CZ | Tele2 (240 07)   | ✅ Funkční |
| Vodafone CZ | Telenor (240 08) | ✅ Funkční |

## Jak přispívat


Pokud nevíte, jak poslat pull request, [založte issue](https://github.com/sixploy/cz-ipv6-roaming/issues/new) a popište v něm:

- se SIM kartou kterého operátora jste cestovali
- v jaké zemi jste IPv6 otestovali
- u jakých operátorů
- s jakým výsledkem

Pokud víte, jak poslat pull request, postupujte například takto:

1. Forkněte repozitář
2. Proveďte změny ve svém forku
   1. přidejte zemi a tabulku s naším operátorem, roamujícím operátorem (ideálně včetně MCC MNC kódu v závorce) a stavem IPv6
   2. doplňte stav IPv6, který jste pozorovali (zkuste například navštívit [test-ipv6.cz](https://test-ipv6.cz) a měření `speedtest.net` vůči serveru českého O2, který používá po IPv6)
   3. Seznam roamingových partnerů T-Mobile je k dispozici [zde](https://www.t-mobile.cz/roaming), nejprve vyberte zemi a pak klikněte na tlačítko `Zobrazit` v sekci `Roamingoví partneři`
   4. Seznam roamingových partnerů Vodafone najdete [tady](https://www.vodafone.cz/roaming/), stačí vyhledat konkrétní zemi 
3. Pošlete pull request

[Seznam MCC kódů](https://en.wikipedia.org/wiki/Mobile_country_code) je na Wikipedii, stejně tak seznam MNC kódů (pro [Evropu](https://en.wikipedia.org/wiki/Mobile_network_codes_in_ITU_region_2xx_(Europe))).

## Seznam přispěvatelů

- [Radek Zajíc](https://github.com/zajdee)
- Radim Friedel

## Licence

Tento seznam je licencován podle [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).
