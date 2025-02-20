---
title: "ZAPping the OWASP Top 10 (2017)"
description: "This document gives an overview of the automatic and manual components provided by OWASP Zed Attack Proxy (ZAP) that are recommended for testing each of the OWASP Top Ten Project 2017 risks."
images:
- https://www.zaproxy.org/img/docs/guides/OWASP-Top-10.png
tags: 
- top10
- guide
type: page
date: "2020-01-30"
addSocialPreview: true
---

This document gives an overview of the automatic and manual components provided by OWASP Zed Attack Proxy (ZAP) that are recommended for testing each of the OWASP Top Ten Project 2017 risks.

For the latest Top Ten see [ZAPping the OWASP Top 10 (2021)](/docs/guides/zapping-the-top-10-2021)

Note that the [OWASP Top Ten Project](https://owasp.org/www-project-top-ten/) risks cover a wide range of underlying vulnerabilities, some of which are not really possible to test for in a completely automated way. 
If a completely automated tool claims to protect you against the full OWASP Top Ten then you can be sure they are being ‘economical with the truth’!

The component links take you to the relevant places in an online version of the ZAP User Guide from which you can learn more. 

|  |  |  |
|--|--|--|
| {{< heading level="5" heading="Common Components" >}}   |  | The 'common components' can be used for pretty much everything, so can be used to help detect all of the Top 10   |
|   | Manual | [Manipulator-in-the-middle proxy](/docs/desktop/start/features/intercept/)   |
|   | Manual | [Manual request](/docs/desktop/ui/dialogs/man_req/) / resend   |
|   | Manual | [Scripts](/docs/desktop/addons/script-console/) |
|   | Manual | [Search](/docs/desktop/ui/tabs/search/)   |
| [{{< heading level="5" heading="A1 Injection" >}}](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A1-Injection) |  | |
|   | Automated | [Active Scan Rules](/docs/desktop/start/features/ascan/) ([Release](/docs/desktop/addons/active-scan-rules/), [Beta*](/docs/desktop/addons/active-scan-rules-beta/), and [Alpha*](/docs/desktop/addons/active-scan-rules-alpha/))   |
|   | Automated | [Advanced SQLInjection Scanner* (Based on SQLMap)](/docs/desktop/addons/advanced-sqlinjection-scanner/)  |
|   | Manual | [Fuzzer](/docs/desktop/addons/fuzzer/), combined with the [FuzzDb*](/docs/desktop/addons/fuzzdb-files/) and [SVN Digger*](/docs/desktop/addons/svn-digger-files/) files |
| [{{< heading level="5" heading="A2 Broken Authentication" >}}](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A2-Broken_Authentication) |  | |
|   | Manual | [HTTP Sessions](/docs/desktop/start/features/httpsessions/) |
|   | Manual | [Spider](/docs/desktop/start/features/spider/)  |
|   | Manual | [Forced Browse](/docs/desktop/addons/forced-browse/)  |
|   | Manual | [Token Generator*](/docs/desktop/addons/token-generator/)   |
|   | Automatic | [Access Control Testing*](/docs/desktop/addons/access-control-testing/) |
| [{{< heading level="5" heading="A3 Sensitive Data Exposure" >}}](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A3-Sensitive_Data_Exposure)   |  | |
|   | Automated | [Active Scan Rules](/docs/desktop/start/features/ascan/) ([Release](/docs/desktop/addons/active-scan-rules/), [Beta*](/docs/desktop/addons/active-scan-rules-beta/), and [Alpha*](/docs/desktop/addons/active-scan-rules-alpha/))   |
|   | Automated | [Passive Scan Rules](/docs/desktop/start/features/pscan/) ([Release](/docs/desktop/addons/passive-scan-rules/), [Beta*](/docs/desktop/addons/passive-scan-rules-beta/), and [Alpha*](/docs/desktop/addons/passive-scan-rules-alpha/))  |
| [{{< heading level="5" heading="A4 XML External Entities (XXE)" >}}](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A4-XML_External_Entities_(XXE)) |  | |
|   | Automatic | [Active Scan Rules](/docs/desktop/start/features/ascan/) ([Release](/docs/desktop/addons/active-scan-rules/), [Beta*](/docs/desktop/addons/active-scan-rules-beta/), and [Alpha*](/docs/desktop/addons/active-scan-rules-alpha/))   |
| [{{< heading level="5" heading="A5 Broken Access Control" >}}](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A5-Broken_Access_Control) |  | |
|   | Automated | [Active Scan Rules](/docs/desktop/start/features/ascan/) ([Release](/docs/desktop/addons/active-scan-rules/), [Beta*](/docs/desktop/addons/active-scan-rules-beta/), and [Alpha*](/docs/desktop/addons/active-scan-rules-alpha/))   |
|   | Automated | [Passive Scan Rules](/docs/desktop/start/features/pscan/) ([Release](/docs/desktop/addons/passive-scan-rules/), [Beta*](/docs/desktop/addons/passive-scan-rules-beta/), and [Alpha*](/docs/desktop/addons/passive-scan-rules-alpha/))  |
|   | Automated | [Access Control Testing*](/docs/desktop/addons/access-control-testing/) |
|   | Manual | [HttpsInfo*](/docs/desktop/addons/https-info/)  |
|   | Manual | [Port Scanner*](/docs/desktop/addons/port-scan/)   |
|   | Manual | [Wappalyzer - Technology detection*](/docs/desktop/addons/technology-detection/) |
| [{{< heading level="5" heading="A6 Security Misconfiguration" >}}](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A6-Security_Misconfiguration)  |  | |
|   | Manual | [Spider](/docs/desktop/start/features/spider/)  |
|   | Manual | [Ajax Spider](/docs/desktop/addons/ajax-spider/)   |
|   | Manual | [Session comparison](/docs/desktop/ui/tlmenu/report/#compare-with-another-session)  |
|   | Manual | [Access Control Testing*](/docs/desktop/addons/access-control-testing/) |
|   | Manual | [HttpsInfo*](/docs/desktop/addons/https-info/)  |
| [{{< heading level="5" heading="A7 Cross-Site Scripting (XSS)" >}}](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A7-Cross-Site_Scripting_(XSS))   |  | |
|   | Automated | [Active Scan Rules](/docs/desktop/start/features/ascan/) ([Release](/docs/desktop/addons/active-scan-rules/))   |
|   | Manual | [Fuzzer](/docs/desktop/addons/fuzzer/), combined with the [FuzzDb*](/docs/desktop/addons/fuzzdb-files/) files  |
| [{{< heading level="5" heading="A8 Insecure Deserialization" >}}](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A8-Insecure_Deserialization) |  | |
|   | Automated | There are two outstanding issues that are relevant to this Top 10 entry: [Insecure deserialization active scanner](https://github.com/zaproxy/zaproxy/issues/4112) & [Java Serialization Handling](https://github.com/zaproxy/zaproxy/issues/4509) |
| [{{< heading level="5" heading="A9 Using Components with Known Vulnerabilities" >}}](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A9-Using_Components_with_Known_Vulnerabilities)  |  | |
|   | Automated | [Passive Scan Rules](/docs/desktop/start/features/pscan/) ([Alpha*](/docs/desktop/addons/passive-scan-rules-alpha/)) and the [Retire.js](https://www.zaproxy.org/docs/desktop/addons/retire.js/) add-on  |
|   | Manual | [Wappalyzer - Technology detection*](/docs/desktop/addons/technology-detection/) |
| [{{< heading level="5" heading="A10 Insufficient Logging & Monitoring" >}}](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A10-Insufficient_Logging%252526Monitoring.html)  |  | |
|   | Automated / Manual | The Spider(s), Active Scanner, Fuzzer, and Access Control addon can all be used to generate traffic and "attacks" which are potential sources/causes for logging and alerting.   |
|   |  | |


&#42; The stared add-ons are not included by default in the full ZAP release but can be downloaded from the ZAP Marketplace via the ‘Manage add-ons’ button on the ZAP main toolbar.

![ZAP Toolbar - Marketplace Button](/img/zap-screenshot-browse-addons.png)
