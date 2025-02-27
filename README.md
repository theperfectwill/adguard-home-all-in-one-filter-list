# AdGuardHome DNS Filter List<a name="adguardhome-dns-filter-list"></a>

______________________________________________________________________

<!-- mdformat-toc start --slug=github --maxlevel=6 --minlevel=1 -->

- [AdGuardHome DNS Filter List](#adguardhome-dns-filter-list)
  - [What Is This?](#what-is-this)
  - [How Can I Use It?](#how-can-i-use-it)
  - [Which Lists Are Combined Here?](#which-lists-are-combined-here)
  - [Do You Curate the Lists?](#do-you-curate-the-lists)
  - [How Often Is This List Updated?](#how-often-is-this-list-updated)
  - [Whitelist Exceptions You Might Want to Make](#whitelist-exceptions-you-might-want-to-make)
    - [Google Fonts](#google-fonts)
    - [Eve Online](#eve-online)
  - [Last Words](#last-words)

<!-- mdformat-toc end -->

______________________________________________________________________

## What Is This?<a name="what-is-this"></a>

This is a DNS blocklist that can be used for AdGuard. (Does not work with Pi-hole)

This list combines more than 80 other lists, including the default lists from
AdGuardHome, into one single list (formatted for Adguard with duplicated removed),
so you don't have to add countless lists to your AdGuardHome, but just this one.

## How Can I Use It?<a name="how-can-i-use-it"></a>

Pretty simple, copy this link
(https://github.com/theperfectwill/adguard-home-all-in-one-filter-list/blob/master/blocklist.txt?raw=true) and
add it to your AdGuard blocklists.

## Which Lists Are Combined Here?<a name="which-lists-are-combined-here"></a>

Which lists I'm using here, you can see in hostlist compiler configuration
» [click here](config.json) « or have a look at the table below.

| Name                                                                                                        | URL                                                                                                                                           |
| ----------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| AdGuard DNS filter                                                                                          | https://adguardteam.github.io/AdGuardSDNSFilter/Filters/filter.txt                                                                            |
| AdGuard MobileFilter                                                                                        | https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/MobileFilter/sections/specific_app.txt                                    |
| AdAway Default Blocklist                                                                                    | https://adaway.org/hosts.txt                                                                                                                  |
| Dan Pollock's List                                                                                          | https://someonewhocares.org/hosts/zero/hosts                                                                                                  |
| WindowsSpyBlocker - Hosts spy rules                                                                         | https://raw.githubusercontent.com/crazy-max/WindowsSpyBlocker/master/data/hosts/spy.txt                                                       |
| Scam Blocklist by DurableNapkin                                                                             | https://raw.githubusercontent.com/durablenapkin/scamblocklist/master/adguard.txt                                                              |
| The Big List of Hacked Malware Web Sites                                                                    | https://raw.githubusercontent.com/mitchellkrogza/The-Big-List-of-Hacked-Malware-Web-Sites/master/hosts                                        |
| Online Malicious URL Blocklist (AdGuard Home)                                                               | https://malware-filter.gitlab.io/malware-filter/urlhaus-filter-agh.txt                                                                        |
| IDN: ABPindo                                                                                                | https://raw.githubusercontent.com/ABPindo/indonesianadblockrules/master/subscriptions/abpindo.txt                                             |
| KOR: YousList                                                                                               | https://raw.githubusercontent.com/yous/YousList/master/hosts.txt                                                                              |
| NOR: Dandelion Sprouts nordiske filtre                                                                      | https://raw.githubusercontent.com/DandelionSprout/adfilt/master/NorwegianExperimentalList%20alternate%20versions/NordicFiltersAdGuardHome.txt |
| Dandelion Sprout's Anti-Malware List (for AdGuard Home, and for AdGuard for Android/Windows' DNS filtering) | https://raw.githubusercontent.com/DandelionSprout/adfilt/master/Alternate%20versions%20Anti-Malware%20List/AntiMalwareAdGuardHome.txt         |
| POL: Polish filters for Pi hole                                                                             | https://raw.githubusercontent.com/MajkiIT/polish-ads-filter/master/polish-pihole-filters/hostfile.txt                                         |
| SWE: Frellwit's Swedish Hosts File                                                                          | https://raw.githubusercontent.com/lassekongo83/Frellwits-filter-lists/master/Frellwits-Swedish-Hosts-File.txt                                 |
| CHN: anti-AD                                                                                                | https://anti-ad.net/easylist.txt                                                                                                              |
| NLD: Easylist                                                                                               | https://easylist-downloads.adblockplus.org/easylistdutch.txt                                                                                  |
| IRN: Unwanted Iranian domains                                                                               | https://raw.githubusercontent.com/DRSDavidSoft/additional-hosts/master/domains/blacklist/unwanted-iranian.txt                                 |
| MKD: Macedonian Pi-hole Blocklist                                                                           | https://raw.githubusercontent.com/cchevy/macedonian-pi-hole-blocklist/master/hosts.txt                                                        |
| BarbBlock                                                                                                   | https://paulgb.github.io/BarbBlock/blacklists/hosts-file.txt                                                                                  |
| Winhelp MVPS Hosts                                                                                          | https://winhelp2002.mvps.org/hosts.txt                                                                                                        |
| uBlock filters - Default                                                                                    | https://raw.githubusercontent.com/uBlockOrigin/uAssets/master/filters/filters.txt                                                             |
| uBlock filters – Badware risks                                                                              | https://raw.githubusercontent.com/uBlockOrigin/uAssets/master/filters/badware.txt                                                             |
| uBlock filters – Privacy                                                                                    | https://raw.githubusercontent.com/uBlockOrigin/uAssets/master/filters/privacy.txt                                                             |
| uBlock filters – Resource abuse                                                                             | https://raw.githubusercontent.com/uBlockOrigin/uAssets/master/filters/resource-abuse.txt                                                      |
| uBlock filters – Unbreak                                                                                    | https://raw.githubusercontent.com/uBlockOrigin/uAssets/master/filters/unbreak.txt                                                             |
| OISD Big List                                                                                               | https://big.oisd.nl                                                                                                                           |
| Lightswitch05 - Ads and Tracking                                                                            | https://www.github.developerdan.com/hosts/lists/ads-and-tracking-extended.txt                                                                 |
| Lightswitch05 - Facebook                                                                                    | https://www.github.developerdan.com/hosts/lists/facebook-extended.txt                                                                         |
| Lightswitch05 - AMP Hosts                                                                                   | https://www.github.developerdan.com/hosts/lists/amp-hosts-extended.txt                                                                        |
| Lightswitch05 - Dating Services                                                                             | https://www.github.developerdan.com/hosts/lists/dating-services-extended.txt                                                                  |
| Lightswitch05 - Tracking Aggressive                                                                         | https://www.github.developerdan.com/hosts/lists/tracking-aggressive-extended.txt                                                              |
| PolishFiltersTeam - KADhosts                                                                                | https://raw.githubusercontent.com/PolishFiltersTeam/KADhosts/master/KADhosts.txt                                                              |
| FadeMind - Hosts Extra (Spam Hosts)                                                                         | https://raw.githubusercontent.com/FadeMind/hosts.extras/master/add.Spam/hosts                                                                 |
| Firebog - Personal Blocklist by WaLLy3K                                                                     | https://v.firebog.net/hosts/static/w3kbl.txt                                                                                                  |
| Firebog - Neohostsbasic                                                                                     | https://v.firebog.net/hosts/neohostsbasic.txt                                                                                                 |
| Firebog - AdGuardDNS                                                                                        | https://v.firebog.net/hosts/AdguardDNS.txt                                                                                                    |
| Firebog - Admiral                                                                                           | https://v.firebog.net/hosts/Admiral.txt                                                                                                       |
| Firebog - Easylist                                                                                          | https://v.firebog.net/hosts/Easylist.txt                                                                                                      |
| Firebog - Prigent Crypto                                                                                    | https://v.firebog.net/hosts/Prigent-Crypto.txt                                                                                                |
| Firebog - Prigent Malware                                                                                   | https://v.firebog.net/hosts/Prigent-Malware.txt                                                                                               |
| Matomo - Referrer Spam Blacklist                                                                            | https://raw.githubusercontent.com/matomo-org/referrer-spam-blacklist/master/spammers.txt                                                      |
| Matomo.org - Referrer Spammers                                                                              | https://raw.githubusercontent.com/matomo-org/referrer-spam-list/master/spammers.txt                                                           |
| VeleSila - yhosts                                                                                           | https://raw.githubusercontent.com/VeleSila/yhosts/master/hosts                                                                                |
| RooneyMcNibNug - PiHole Stuff (SNAFU)                                                                       | https://raw.githubusercontent.com/RooneyMcNibNug/pihole-stuff/master/SNAFU.txt                                                                |
| anudeepND - Adservers                                                                                       | https://raw.githubusercontent.com/anudeepND/blacklist/master/adservers.txt                                                                    |
| anudeepND - Facebook                                                                                        | https://raw.githubusercontent.com/anudeepND/blacklist/master/facebook.txt                                                                     |
| Ad filter list by Disconnect                                                                                | https://s3.amazonaws.com/lists.disconnect.me/simple_ad.txt                                                                                    |
| Peter Lowe's List                                                                                           | https://pgl.yoyo.org/adservers/serverlist.php?hostformat=adblockplus&showintro=1&mimetype=plaintext                                           |
| Perflyst and Dandelion Sprout's Smart-TV Blocklist                                                          | https://raw.githubusercontent.com/Perflyst/PiHoleBlocklist/master/SmartTV-AGH.txt                                                             |
| Spam404 - Main Blacklist                                                                                    | https://raw.githubusercontent.com/Spam404/lists/master/main-blacklist.txt                                                                     |
| Spam404 - Adblock List                                                                                      | https://raw.githubusercontent.com/Spam404/lists/master/adblock-list.txt                                                                       |
| Game Console Adblock List                                                                                   | https://raw.githubusercontent.com/DandelionSprout/adfilt/master/GameConsoleAdblockList.txt                                                    |
| NoCoin Filter Lis                                                                                           | https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/hosts.txt                                                              |
| VNM: ABPVN List                                                                                             | https://abpvn.com/android/abpvn.txt                                                                                                           |
| FadeMind - UncheckyAds                                                                                      | https://raw.githubusercontent.com/FadeMind/hosts.extras/master/UncheckyAds/hosts                                                              |
| FadeMind - Additional Risks                                                                                 | https://raw.githubusercontent.com/FadeMind/hosts.extras/master/add.Risk/hosts                                                                 |
| bigdargon - hostsVN                                                                                         | https://raw.githubusercontent.com/bigdargon/hostsVN/master/hosts                                                                              |
| jdlingyu - ad-wars                                                                                          | https://raw.githubusercontent.com/jdlingyu/ad-wars/master/hosts                                                                               |
| Threat-Intel                                                                                                | https://osint.digitalside.it/Threat-Intel/lists/latestdomains.txt                                                                             |
| ethanr - DNS-Blacklists                                                                                     | https://bitbucket.org/ethanr/dns-blacklists/raw/8575c9f96e5b4a1308f2f12394abd86d0927a4a0/bad_lists/Mandiant_APT1_Report_Appendix_D.txt        |
| NoTrack Malware Blocklist                                                                                   | https://gitlab.com/quidsup/notrack-blocklists/raw/master/notrack-malware.txt                                                                  |
| abuse.ch URLhaus Host file                                                                                  | https://urlhaus.abuse.ch/downloads/hostfile/                                                                                                  |
| StevenBlack - Hosts                                                                                         | https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts                                                                              |
| Adblock Warning Removal List                                                                                | https://easylist-downloads.adblockplus.org/antiadblockfilters.txt                                                                             |
| ABP filters                                                                                                 | https://easylist-downloads.adblockplus.org/abp-filters-anti-cv.txt                                                                            |
| AdGuard CNAME disguised trackers list                                                                       | https://raw.githubusercontent.com/AdguardTeam/cname-trackers/master/data/combined_disguised_trackers.txt                                      |
| Easylist Cookie List                                                                                        | https://secure.fanboy.co.nz/fanboy-cookiemonster.txt                                                                                          |
| EasyPrivacy                                                                                                 | https://easylist.to/easylist/easyprivacy.txt                                                                                                  |
| NextDNS CNAME Cloaking Blocklist                                                                            | https://raw.githubusercontent.com/nextdns/cname-cloaking-blocklist/master/domains                                                             |
| NextDNS Privacy - Alexa                                                                                     | https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/alexa                                                          |
| NextDNS Privacy - Apple                                                                                     | https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/apple                                                          |
| NextDNS Privacy - Huawei                                                                                    | https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/huawei                                                         |
| NextDNS Privacy - Roku                                                                                      | https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/roku                                                           |
| NextDNS Privacy - Samsung                                                                                   | https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/samsung                                                        |
| NextDNS Privacy - Sonos                                                                                     | https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/sonos                                                          |
| NextDNS Privacy - Windows                                                                                   | https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/windows                                                        |
| NextDNS Privacy - Xiaomi                                                                                    | https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/xiaomi                                                         |
| First-party trackers host list                                                                              | https://hostfiles.frogeye.fr/firstparty-trackers-hosts.txt                                                                                    |
| Firebog - Easyprivacy                                                                                       | https://v.firebog.net/hosts/Easyprivacy.txt                                                                                                   |
| Firebog - Prigent-Ads                                                                                       | https://v.firebog.net/hosts/Prigent-Ads.txt                                                                                                   |
| FadeMind - hosts.extras/add.2o7Net                                                                          | https://raw.githubusercontent.com/FadeMind/hosts.extras/master/add.2o7Net/hosts                                                               |
| Malvertising list by Disconnect                                                                             | https://s3.amazonaws.com/lists.disconnect.me/simple_malvertising.txt                                                                          |
| Phishing URL Blocklist (AdGuard Home)                                                                       | https://malware-filter.gitlab.io/malware-filter/phishing-filter-agh.txt                                                                       |
| HaGeZi's Multi DNS Blocklist                                                                                | https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/multi.txt                                                                |
| HaGeZi's DoH/VPN/TOR/Proxy Bypass DNS Blocklist                                                             | https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/doh-vpn-proxy-bypass.txt                                                 |
| HaGeZi's Fake DNS Blocklist                                                                                 | https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/fake.txt                                                                 |
| HaGeZi's Threat Intelligence Feeds DNS Blocklist                                                            | https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/tif.txt                                                                  |
| FR: French filters RedFlagDomains                                                                           | https://dl.red.flag.domains/red.flag.domains.txt                                                                                              |

## Do You Curate the Lists?<a name="do-you-curate-the-lists"></a>

Absolutely not.

All these lists are considered 3rd party from my point of view. I have no influence
over them at all. All I do is combine the lists I was using into one single list, so
my list of blocklists isn't massive. (That was a lot of lists in one sentence ...)

## How Often Is This List Updated?<a name="how-often-is-this-list-updated"></a>

Once a day

## Whitelist Exceptions You Might Want to Make<a name="whitelist-exceptions-you-might-want-to-make"></a>

### Google Fonts<a name="google-fonts"></a>

As stated [here](https://github.com/lightswitch05/hosts#google-fonts) from one of
the lists I am using, you might have to whitelist `fonts.gstatic.com`. To do so, add
the following to your whitelist:

```plainext
@@||fonts.gstatic.com^$important
```

### Eve Online<a name="eve-online"></a>

If you are playing Eve Online by any chance, you also might want to add the
following line to your custom filter rules:

```plaintext
@@||extccp.com^$important
```

## Last Words<a name="last-words"></a>

You are free to use this list, but I can give you no guarantee for it since none of
the lists combined here is managed by me.

If you want to create your own combined list, feel free to fork this repository and
change the host list compiler configuration included to start your own repo. To
compile the host list, use
[AdGuard's HostlistCompiler](https://github.com/AdguardTeam/HostlistCompiler).
