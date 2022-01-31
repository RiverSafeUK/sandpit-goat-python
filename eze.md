  
# Eze Report Results


## Summary  ![tools](https://img.shields.io/static/v1?style=plastic&label=Tools_executed&message=5&color=blue)
---

Branch tested: main


![critical](https://img.shields.io/static/v1?style=plastic&label=critical&message=0&color=red)
![high](https://img.shields.io/static/v1?style=plastic&label=high&message=3&color=orange)
![medium](https://img.shields.io/static/v1?style=plastic&label=medium&message=7&color=yellow)
![low](https://img.shields.io/static/v1?style=plastic&label=low&message=2&color=lightgrey)
            

## Vulnerabilities
---


    [python-piprot] Vulnerabilities
    =================================
    TOOL REPORT: [github] python-piprot (scan duration: 0.3 seconds)
        total: 1 (high:1)
        ignored: 1 (none:1)

        [HIGH DEPENDENCY] : requests (2.4.0)
        overview: requests (2.4.0) is 2686 days out of date. Latest is 2.27.1
        recommendation: requests (2.4.0) 2686 days out of date. update to a newer version, latest version: 2.27.1

        [NONE DEPENDENCY] : requests (2.4.0)
        overview: requests (2.4.0) is 2686 days out of date. Latest is 2.27.1
        recommendation: update requests (2.4.0) to a newer version, current version is 23 minor versions out of date. Latest is 2.27.1


    [python-safety] Vulnerabilities
    =================================
    TOOL REPORT: [github] python-safety (scan duration: 4.4 seconds)
        total: 3 (medium:3, warnings:true)
        ignored: 9 (low:1, na:8, warnings:true)

        [MEDIUM DEPENDENCY] : pip (1.3.0)
        overview: A flaw was found in python-pip in the way it handled Unicode separators in git references. A remote attacker could possibly use this issue to install a different revision on a repository. The highest threat from this vulnerability is to data integrity. This is fixed in python-pip version 21.1.
        cve: CVE-2021-3572
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <21.1

        [MEDIUM DEPENDENCY] : pip (1.3.0)
        overview: The mirroring support (-M, --use-mirrors) in Python Pip before 1.5 uses insecure DNS querying and authenticity checks which allows attackers to perform man-in-the-middle attacks.
        cve: CVE-2013-5123
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <1.5

        [MEDIUM DEPENDENCY] : pip (1.3.0)
        overview: The resolve_redirects function in sessions.py in requests 2.1.0 through 2.5.3 allows remote attackers to conduct session fixation attacks via a cookie without a host value in a redirect.
        cve: CVE-2015-2296
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <6.1.0

        [LOW DEPENDENCY] : pip (1.3.0)
        overview: pip 1.3 through 1.5.6 allows local users to cause a denial of service (prevention of package installation) by creating a /tmp/pip-build-* file for another user.
        cve: CVE-2014-8991
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <6.0

        [NA DEPENDENCY] : pip (1.3.0)
        overview: Pip version 21.1 stops splitting on unicode separators in git references, which could be maliciously used to install a different revision on the repository. 
https://github.com/pypa/pip/issues/9827
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <21.1

        [NA DEPENDENCY] : pip (1.3.0)
        overview: The pip package before 19.2 for Python allows Directory Traversal when a URL is given in an install command, because a Content-Disposition header can have ../ in a filename, as demonstrated by overwriting the /root/.ssh/authorized_keys file. This occurs in _download_http_url in _internal/download.py.
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <19.2

        [NA DEPENDENCY] : pip (1.3.0)
        overview: The resolve_redirects function in sessions.py in requests 2.1.0 through 2.5.3 allows remote attackers to conduct session fixation attacks via a cookie without a host value in a redirect.
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <6.1.0

        [NA DEPENDENCY] : pip (1.3.0)
        overview: The urllib3 library 1.26.x before 1.26.4 for Python omits SSL certificate validation in some cases involving HTTPS to HTTPS proxies. The initial connection to the HTTPS proxy (if an SSLContext isn't given via proxy_config) doesn't verify the hostname of the certificate. This means certificates for different servers that still validate properly with the default urllib3 SSLContext will be silently accepted.
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <21.1

        [NA DEPENDENCY] : pip (1.3.0)
        overview: pip 1.4 includes a security patch to pip's ssl support related to certificate DNS wildcard matching.
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <1.4

        [NA DEPENDENCY] : requests (2.4.0)
        overview: The Requests package through 2.19.1 sends an HTTP Authorization header to an http URI upon receiving a same-hostname https-to-http redirect, which makes it easier for remote attackers to discover credentials by sniffing the network.
        recommendation: Update requests (2.4.0) to a non vulnerable version, vulnerable versions: <=2.19.1

        [NA DEPENDENCY] : requests (2.4.0)
        overview: The resolve_redirects function in sessions.py in requests 2.1.0 through 2.5.3 allows remote attackers to conduct session fixation attacks via a cookie without a host value in a redirect.
        recommendation: Update requests (2.4.0) to a non vulnerable version, vulnerable versions: >=2.1,<=2.5.3

        [NA DEPENDENCY] : requests (2.4.0)
        overview: requests 2.6.0 fixes handling of cookies on redirect. Previously a cookie without a host value set would use the hostname for the redirected URL exposing requests users to session fixation attacks and potentially cookie stealing.
        recommendation: Update requests (2.4.0) to a non vulnerable version, vulnerable versions: <2.6.0


    [python-cyclonedx] Vulnerabilities
    =================================
    TOOL REPORT: [github] python-cyclonedx (scan duration: 7.1 seconds)
        components: 2 (License :: OSI Approved :: MIT License:1, License :: OSI Approved :: Apache Software License:1)
        total: 6 (high:2, medium:3, low:1, warnings:true)
        ignored: 0 

        [HIGH DEPENDENCY] : The Requests package before 2.20.0 for Python sends an HTTP Authorization header to an http URI upon receiving a same-hostname https-to-http redirect, which makes it easier for remote attackers to discover credentials by sniffing the network.
        overview: 
        PYSEC: PYSEC-2018-28
        CVE: CVE-2018-18074
        recommendation: Update package to non-vulnerable version 2.20.0

        [HIGH DEPENDENCY] : The pip package before 19.2 for Python allows Directory Traversal when a URL is given in an install command, because a Content-Disposition header can have ../ in a filename, as demonstrated by overwriting the /root/.ssh/authorized_keys file. This occurs in _download_http_url in _internal/download.py.
        overview: 
        PYSEC: PYSEC-2020-173
        CVE: CVE-2019-20916
        recommendation: Update package to non-vulnerable version 19.2

        [MEDIUM DEPENDENCY] : A flaw was found in python-pip in the way it handled Unicode separators in git references. A remote attacker could possibly use this issue to install a different revision on a repository. The highest threat from this vulnerability is to data integrity. This is fixed in python-pip version 21.1.
        overview: 
        PYSEC: PYSEC-2021-437
        CVE: CVE-2021-3572
        recommendation: Update package to non-vulnerable version 21.1

        [MEDIUM DEPENDENCY] : The mirroring support (-M, --use-mirrors) in Python Pip before 1.5 uses insecure DNS querying and authenticity checks which allows attackers to perform man-in-the-middle attacks.
        overview: 
        PYSEC: PYSEC-2019-160
        CVE: CVE-2013-5123
        recommendation: Update package to non-vulnerable version 1.5

        [MEDIUM DEPENDENCY] : The resolve_redirects function in sessions.py in requests 2.1.0 through 2.5.3 allows remote attackers to conduct session fixation attacks via a cookie without a host value in a redirect.
        overview: 
        PYSEC: PYSEC-2015-17
        CVE: CVE-2015-2296
        recommendation: Update package to non-vulnerable version 2.6.0

        [LOW DEPENDENCY] : pip 1.3 through 1.5.6 allows local users to cause a denial of service (prevention of package installation) by creating a /tmp/pip-build-* file for another user.
        overview: 
        PYSEC: PYSEC-2014-11
        CVE: CVE-2014-8991
        recommendation: Update package to non-vulnerable version 6.0


    [trufflehog] Vulnerabilities
    =================================
    TOOL REPORT: [github] trufflehog (scan duration: 0.4 seconds)
        total: 2 (medium:1, low:1)
        ignored: 0 

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in src/super-insecure-lib.py
        recommendation: Investigate 'src/super-insecure-lib.py' Line 3 for 'High Entropy' strings Full Match: INSECURE_SECRET_RSA_KEY = "ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR"
        file: src/super-insecure-lib.py (line 3)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in src/super-insecure-lib.py
        recommendation: Investigate 'src/super-insecure-lib.py' Line 5 for 'Password in URL' strings Full Match: INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = "https://admin:god@hackers.com"
        file: src/super-insecure-lib.py (line 5)


## Bill of Materials
---

![components](https://img.shields.io/static/v1?style=plastic&label=components&message=2&color=blue)

### [python-cyclonedx] SBOM
---

| type    | name     | version | license    | license type | description |
| ------- | -------- | ------- | ---------- | ------------ | ----------- |
| library | pip      | 1.3.0   | MIT        | permissive   |             |
| library | requests | 2.4.0   | Apache-2.0 | permissive   |             |

## Warnings
---

    [python-bandit] Warnings
    =================================
    {"filename": "app", "reason": "No such file or directory"}

    [python-safety] Warnings
    =================================
    Warning: unpinned requirement 'click' found in requirements.txt, unable to check.
    

    [python-cyclonedx] Warnings
    =================================
    Warning: unpinned requirement 'click' found in requirements.txt, unable to check

