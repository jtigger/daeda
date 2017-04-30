# Selecting A VPN Service

The VPN Service industry is infested with misinformation and bad actors:
- most VPN review sites you read are paid-for marketing;
- law enforcement looking for ways to catch cyber-criminals create "honey pot" services that look just like legitimate businesses;
- hackers look for ways to conduct so-called "Man in the Middle" attacks will try to lure you in to using their service so _they_ can capture your private information.

Navigating this jungle is extremely difficult for even the tech savvy.  Currently (circa early 2017), this is the domain of security experts.

Thankfully, there are experts who are willing to share their homework with the rest of us. One of the best sources of information about VPN Services is at [That One Privacy Site](https://thatoneprivacysite.net/vpn-section/).
This site is maintained by one person (aptly goes by the moniker [That One Privacy Guy](https://twitter.com/ThatPrivacyGuy); I'll refer to her/him by the acronym TOPG).  She/he has dedicated 1,000+ hours and put to use her/his considerable skills in compiling this information.

What follows is a guide to interpreting her/his research in terms that the rest of us can relate to.

If you find TOPG's work useful, please consider making [a small donation](https://thatoneprivacysite.net/donate/).

> **NOTE: VPN services are generally incompatible with streaming, today.**
>
>Many households have turned to on-demand streaming services like Netflix, Hulu and Vudu to replace their television watching wants.
>
> As of early 2017, many of these services refuse to stream over VPN-encrypted connections.  For the streaming service's part, they are trying to deliver content only in the geographic region they were licensed to do so.  Using a VPN service you can be in China yet appear to be sitting in New York.  Netflix can't tell the difference between someone just protecting their personal privacy from someone trying to circumvent geographical licensing restrictions.
>
>As a result, to stream over VPN, you would have to take extraordinary steps to conceal the fact that you're using a VPN; a setup out of scope here.


## Finding the right VPN service for you

TOPG has compiled her/his research into a Google spreadsheet. The best way to find the VPN service fit for you is to filter and sort that spreadsheet.  She/he also includes an accessible and thoughtful guide on [how to choose a VPN service](https://thatoneprivacysite.net/choosing-the-best-vpn-for-you/).


Here is the most straight-forward way to do that:

1. Go to the spreadsheet: https://docs.google.com/spreadsheets/d/1L72gHJ5bTq0Djljz0P-NCAaURrXwsR1MsLpVmAt3bwg/edit
1. In the spreadsheet: Open the `File` menu, then select `Make a copy...`
1. In your copy: select rows 5 through the last row; select `Data` then `Filter`
   - You should see the filter icon (i.e. a striped triangle) next to each header in row 5.

Use the following guidance to narrow down the list.

**... if you want to weed-out VPN service vendors with demonstrated questionable practices...**

require credibility in service description:
- `Contradictory Logging Policies` _(column BE)_ — uncheck `Yes`, if present.

_(rationale: you are trusting the VPN vendor will act in good faith.  If they are not impeccable with their words, they are likely not so with their actions.)_

**... if you want to prevent your ISP from seeing _any_ your Internet traffic ...**

require DNS and IPv6 leak protection:
- `1st Party DNS Servers` _(column Y)_ — ensure only `Yes` is checked.
- `IPv6 Supported/Blocked`_(column Z)_ — ensure only `Yes` is checked.

_(rationale: without these protections, some of your traffic may be visible even with VPN turned on.  This may be enough to correlate back to your encrypted traffic.  Any VPN service with an interest in providing privacy will **explicitly** indicate these protections.)_

**... if you want to be pretty darn sure your Internet traffic will never shared without your permission ...**

require your VPN service to explicitly not retain logs:
- `Logging`_(column C)_ — ensure only `0`, `0.5`, and `1` are checked.
- `Activity`/`Traffic`_(column O)_ — uncheck `Yes`, if present.
- `Activity`/`DNS Requests`_(column P)_ — uncheck `Yes`, if present.
- `Connection`/`Timestamps`_(column Q)_ — uncheck `Yes`, if present.
- `Connection`/`Bandwidth`_(column R)_ — uncheck `Yes`, if present.
- `Connection`/`IP Address`_(column S)_ — uncheck `Yes`, if present.

_(rationale: VPN services do not **need** to retain data to function.  A blank in one of these columns indicates that TOPG could not **explicitly confirm** the VPN service does not log that type of data — but if the service does not log most data, it likely does not log any.)_

**... if you see the use of hyperbolic language as an indicator of dishonesty ...**

- `Falsely Claims Service is 100% Effective` _(column BF)_ — uncheck `Yes`, if present.

_(rationale: there are no true absolutes in security and privacy.  This is almost always true: if a nation-state wishes to snoop on you, they have the resources to do so.  Claiming otherwise is misleading.)_


## Giving back

- Consider whether you would have found your VPN Service without this help.
- Take stock in the peace of mind you have using it ... would that have been possible without this help?
- Remind yourself of the [Bystander Effect](https://en.wikipedia.org/wiki/Bystander_effect).
- Given what this person has already given away, it be a _good_ thing if she/he had some extra cash to cover her/his costs and provide resources to do more?
- security is a moving target. Supporting this effort means that not only can you make an informed choice today, but likely maintain that confidence as the landscape changes.

## Caveats

### Assessments are (properly) conservative... and this can be surprising at times.

TOPG conservatively assesses available data.  Reviewing assessments, her/his stance may seem a bit pedantic.  Of course when dealing with security and privacy, this is the proper stance.

There may be a number of legitimate VPN services that get low scores in a particular subject because the exact nature of the VPN service's claim is not precise enough.

A common example is logging.  If a VPN service's FAQ includes:

> Q: Do you keep logs?  A:No.  Never have.  Never will.

no assessment can be made because it does not differentiate between traffic logs, DNS logs, connection timestamp, bandwidth usage and IP address logging.  Where the VPN service _is_ explicit, TOPG will record that fact.

This can frustrate some (especially representatives of the service or affiliates).  From your perspective as the consumer of this data, the pedantic reading is most welcome.

Here's an exemplary way to describe logging practices: https://www.mullvad.net/blog/2017/1/13/clarifying-our-no-logging-policy/

----

# Further Reading/Research on VPN Services

- Quick and dirty VPN advice: https://free-dissociation.com/blog/posts/2017/03/quick-and-dirty-vpn-advice/
- Most VPN services are terrible — https://gist.github.com/kennwhite/1f3bc4d889b02b35d8aa
- vpwns: Virtual Pwned Networks — https://www.usenix.org/system/files/conference/foci12/foci12-final8.pdf

- VPN Vendors:
  - Private Internet Access (PIA)
    - public proof the do not keep logs: https://www.scribd.com/doc/303226103/Fake-bomb-threat-arrest
    - statement they do not keep logs: https://helpdesk.privateinternetaccess.com/hc/en-us/articles/219457547-Do-you-log-the-traffic-of-your-users-
  - Cloak (src: rmoran)
