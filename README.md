# OWASP_WSTG_ASVS
Spreadsheet with vulnerabilites from OWASP's WSTG and ASVS

The idea behind this project is to create a spreadsheet with vulnerabilities so that penetration testers use it to import them in automatic reporting tools. (such as [pwndoc-ng](https://github.com/pwndoc-ng/pwndoc-ng)) 



preview


I've uploaded the spreadsheet to Google sheets aswell: https://docs.google.com/spreadsheets/d/1jj7ESXg9ks-97XiHbdcWJbfsims2d3MP2MxSuNdesWk/edit?usp=sharing


# How is each field built?

I've taken the OWASP WSTG as a base and then tried to add vulnerabilities that were missing in WSTG but were present in ASVS. Here are the fields of the spreadsheet:

+ Recommended CVSSv3: CVSSv3.1 recommended vector. Note that this is just a hint and should not be used as-is. Each vulnerability depends heavily on the context, but it is nice that the reporting tools have at least a template.
+ OWASP ASVS: OWASP ASVS code for the vuln. **NOTE**: there is a mapping between WSTG and ASVS that were made taking inspiration from https://github.com/jeremychoi/owasp-asvs-wstg-checklist. Every mapping may not be the same as in this repo, though. 
+ OWASP WSTG: OWASP WSTG code for the vuln.
+ Category: Category from OWASP WSTG.
+ Title: titles are made by hand.
+ CWE: Associated CWE for the vuln. I tried that every vuln has at least one code. (See Impact field) 
+ Description: description of each vuln was made by hand.
+ Impact codes: Each CWE has an impact section (take https://cwe.mitre.org/data/definitions/299.html for example and scroll down to the "Common consequences" section, you'll see it). I've made an inventory of CWE's impacts so that they can be repeated. This inventory is in the Impact_ENG sheet and each has an ID. These IDs are the Impact codes.
+ Impact: The text from the impact itself is taken from the impact inventory 
+ Remediation: remediation of each vuln was made by hand.
+ References: The references are either the CWE of the link for WSTG.

## Limitations

+ I know that OWASP WSTG is aimed to technical profiles and ASVS more to a vulnerability management profile, but I feel there is a gap when penetration testers need to report findings to both high level profiles and technical profiles. Vulnerabilities repeat all the time. This project is made for saving time, not having to write vulnerabilites every time.
+ The mapping between OWASP WSTG and ASVS is not perfect, and probably it will neve be because the scope for the projects is different, but I've made it following a best-effort approach. The same happens with associated CWE codes.



# Languages

Available, so far in:

+ English
+ Spanish


# Contributions

I know that there will be aspects that could be polished and are not accurate 100%. If you think, so, contribute please =)
Feel free to open issues and pull requests =)
