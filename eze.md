  
# Eze Report Results


## Summary  ![tools](https://img.shields.io/static/v1?style=plastic&label=Tools&message=5&color=blue)
---


![critical](https://img.shields.io/static/v1?style=plastic&label=critical&message=0&color=red)
![high](https://img.shields.io/static/v1?style=plastic&label=high&message=4&color=orange)
![medium](https://img.shields.io/static/v1?style=plastic&label=medium&message=53&color=yellow)
![low](https://img.shields.io/static/v1?style=plastic&label=low&message=6&color=lightgrey)
            
<b>Branch tested: </b>main

<b>Tools executed: </b>

* python-piprot (SCA)
            
* python-bandit (SAST)
            
* python-safety (SAST)
            
* python-cyclonedx (SBOM)
            
* trufflehog (SECRET)
            

## Vulnerabilities
---


    [python-piprot] Vulnerabilities
    =================================
    TOOL REPORT: [github] python-piprot (scan duration: 0.3 seconds)
        total: 6 (high:2, medium:4)
        ignored: 4 (none:4)

        [HIGH DEPENDENCY] : requests (2.4.0)
        overview: requests (2.4.0) is 2686 days out of date. Latest is 2.27.1
        recommendation: requests (2.4.0) 2686 days out of date. update to a newer version, latest version: 2.27.1

        [HIGH DEPENDENCY] : requests (2.4.0)
        overview: requests (2.4.0) is 2686 days out of date. Latest is 2.27.1
        recommendation: requests (2.4.0) 2686 days out of date. update to a newer version, latest version: 2.27.1

        [MEDIUM DEPENDENCY] : black (20.8b1)
        overview: black (20.8b1) is 521 days out of date. Latest is 22.1.0
        recommendation: black (20.8b1) 521 days out of date. update to a newer version, latest version: 22.1.0

        [MEDIUM DEPENDENCY] : pytest-snapshot (0.5.0)
        overview: pytest-snapshot (0.5.0) is 385 days out of date. Latest is 0.8.1
        recommendation: pytest-snapshot (0.5.0) 385 days out of date. update to a newer version, latest version: 0.8.1

        [MEDIUM DEPENDENCY] : pytest (6.2.2)
        overview: pytest (6.2.2) is 382 days out of date. Latest is 7.0.1
        recommendation: pytest (6.2.2) 382 days out of date. update to a newer version, latest version: 7.0.1

        [MEDIUM DEPENDENCY] : pytest (6.2.2)
        overview: pytest (6.2.2) is 382 days out of date. Latest is 7.0.1
        recommendation: update pytest (6.2.2) to a newer version, current version is 1 major versions out of date. Latest is 7.0.1

        [NONE DEPENDENCY] : black (20.8b1)
        overview: black (20.8b1) is 521 days out of date. Latest is 22.1.0
        recommendation: update black (20.8b1) to a newer version. Latest is 22.1.0

        [NONE DEPENDENCY] : pytest-snapshot (0.5.0)
        overview: pytest-snapshot (0.5.0) is 385 days out of date. Latest is 0.8.1
        recommendation: update pytest-snapshot (0.5.0) to a newer version, current version is 3 minor versions out of date. Latest is 0.8.1

        [NONE DEPENDENCY] : requests (2.4.0)
        overview: requests (2.4.0) is 2686 days out of date. Latest is 2.27.1
        recommendation: update requests (2.4.0) to a newer version, current version is 23 minor versions out of date. Latest is 2.27.1

        [NONE DEPENDENCY] : requests (2.4.0)
        overview: requests (2.4.0) is 2686 days out of date. Latest is 2.27.1
        recommendation: update requests (2.4.0) to a newer version, current version is 23 minor versions out of date. Latest is 2.27.1


    [python-safety] Vulnerabilities
    =================================
    TOOL REPORT: [github] python-safety (scan duration: 6.0 seconds)
        total: 6 (medium:6, warnings:true)
        ignored: 18 (low:2, na:16, warnings:true)

        [MEDIUM DEPENDENCY] : pip (1.3.0)
        overview: A flaw was found in python-pip in the way it handled Unicode separators in git references. A remote attacker could possibly use this issue to install a different revision on a repository. The highest threat from this vulnerability is to data integrity. This is fixed in python-pip version 21.1.
        cve: CVE-2021-3572
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <21.1

        [MEDIUM DEPENDENCY] : pip (1.3.0)
        overview: A flaw was found in python-pip in the way it handled Unicode separators in git references. A remote attacker could possibly use this issue to install a different revision on a repository. The highest threat from this vulnerability is to data integrity. This is fixed in python-pip version 21.1.
        cve: CVE-2021-3572
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <21.1

        [MEDIUM DEPENDENCY] : pip (1.3.0)
        overview: The mirroring support (-M, --use-mirrors) in Python Pip before 1.5 uses insecure DNS querying and authenticity checks which allows attackers to perform man-in-the-middle attacks.
        cve: CVE-2013-5123
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <1.5

        [MEDIUM DEPENDENCY] : pip (1.3.0)
        overview: The mirroring support (-M, --use-mirrors) in Python Pip before 1.5 uses insecure DNS querying and authenticity checks which allows attackers to perform man-in-the-middle attacks.
        cve: CVE-2013-5123
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <1.5

        [MEDIUM DEPENDENCY] : pip (1.3.0)
        overview: The resolve_redirects function in sessions.py in requests 2.1.0 through 2.5.3 allows remote attackers to conduct session fixation attacks via a cookie without a host value in a redirect.
        cve: CVE-2015-2296
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <6.1.0

        [MEDIUM DEPENDENCY] : pip (1.3.0)
        overview: The resolve_redirects function in sessions.py in requests 2.1.0 through 2.5.3 allows remote attackers to conduct session fixation attacks via a cookie without a host value in a redirect.
        cve: CVE-2015-2296
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <6.1.0

        [LOW DEPENDENCY] : pip (1.3.0)
        overview: pip 1.3 through 1.5.6 allows local users to cause a denial of service (prevention of package installation) by creating a /tmp/pip-build-* file for another user.
        cve: CVE-2014-8991
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <6.0

        [LOW DEPENDENCY] : pip (1.3.0)
        overview: pip 1.3 through 1.5.6 allows local users to cause a denial of service (prevention of package installation) by creating a /tmp/pip-build-* file for another user.
        cve: CVE-2014-8991
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <6.0

        [NA DEPENDENCY] : pip (1.3.0)
        overview: Pip 21.1 updates its dependency 'urllib3' to v1.26.4 due to security issues.
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <21.1

        [NA DEPENDENCY] : pip (1.3.0)
        overview: Pip 21.1 updates its dependency 'urllib3' to v1.26.4 due to security issues.
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <21.1

        [NA DEPENDENCY] : pip (1.3.0)
        overview: Pip version 21.1 stops splitting on unicode separators in git references, which could be maliciously used to install a different revision on the repository. 
https://github.com/pypa/pip/issues/9827
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <21.1

        [NA DEPENDENCY] : pip (1.3.0)
        overview: Pip version 21.1 stops splitting on unicode separators in git references, which could be maliciously used to install a different revision on the repository. 
https://github.com/pypa/pip/issues/9827
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <21.1

        [NA DEPENDENCY] : pip (1.3.0)
        overview: The pip package before 19.2 for Python allows Directory Traversal when a URL is given in an install command, because a Content-Disposition header can have ../ in a filename, as demonstrated by overwriting the /root/.ssh/authorized_keys file. This occurs in _download_http_url in _internal/download.py.
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <19.2

        [NA DEPENDENCY] : pip (1.3.0)
        overview: The pip package before 19.2 for Python allows Directory Traversal when a URL is given in an install command, because a Content-Disposition header can have ../ in a filename, as demonstrated by overwriting the /root/.ssh/authorized_keys file. This occurs in _download_http_url in _internal/download.py.
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <19.2

        [NA DEPENDENCY] : pip (1.3.0)
        overview: The resolve_redirects function in sessions.py in requests 2.1.0 through 2.5.3 allows remote attackers to conduct session fixation attacks via a cookie without a host value in a redirect.
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <6.1.0

        [NA DEPENDENCY] : pip (1.3.0)
        overview: The resolve_redirects function in sessions.py in requests 2.1.0 through 2.5.3 allows remote attackers to conduct session fixation attacks via a cookie without a host value in a redirect.
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <6.1.0

        [NA DEPENDENCY] : pip (1.3.0)
        overview: pip 1.4 includes a security patch to pip's ssl support related to certificate DNS wildcard matching.
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <1.4

        [NA DEPENDENCY] : pip (1.3.0)
        overview: pip 1.4 includes a security patch to pip's ssl support related to certificate DNS wildcard matching.
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <1.4

        [NA DEPENDENCY] : requests (2.4.0)
        overview: The Requests package through 2.19.1 sends an HTTP Authorization header to an http URI upon receiving a same-hostname https-to-http redirect, which makes it easier for remote attackers to discover credentials by sniffing the network.
        recommendation: Update requests (2.4.0) to a non vulnerable version, vulnerable versions: <=2.19.1

        [NA DEPENDENCY] : requests (2.4.0)
        overview: The Requests package through 2.19.1 sends an HTTP Authorization header to an http URI upon receiving a same-hostname https-to-http redirect, which makes it easier for remote attackers to discover credentials by sniffing the network.
        recommendation: Update requests (2.4.0) to a non vulnerable version, vulnerable versions: <=2.19.1

        [NA DEPENDENCY] : requests (2.4.0)
        overview: The resolve_redirects function in sessions.py in requests 2.1.0 through 2.5.3 allows remote attackers to conduct session fixation attacks via a cookie without a host value in a redirect.
        recommendation: Update requests (2.4.0) to a non vulnerable version, vulnerable versions: >=2.1,<=2.5.3

        [NA DEPENDENCY] : requests (2.4.0)
        overview: The resolve_redirects function in sessions.py in requests 2.1.0 through 2.5.3 allows remote attackers to conduct session fixation attacks via a cookie without a host value in a redirect.
        recommendation: Update requests (2.4.0) to a non vulnerable version, vulnerable versions: >=2.1,<=2.5.3

        [NA DEPENDENCY] : requests (2.4.0)
        overview: requests 2.6.0 fixes handling of cookies on redirect. Previously a cookie without a host value set would use the hostname for the redirected URL exposing requests users to session fixation attacks and potentially cookie stealing.
        recommendation: Update requests (2.4.0) to a non vulnerable version, vulnerable versions: <2.6.0

        [NA DEPENDENCY] : requests (2.4.0)
        overview: requests 2.6.0 fixes handling of cookies on redirect. Previously a cookie without a host value set would use the hostname for the redirected URL exposing requests users to session fixation attacks and potentially cookie stealing.
        recommendation: Update requests (2.4.0) to a non vulnerable version, vulnerable versions: <2.6.0


    [python-cyclonedx] Vulnerabilities
    =================================
    TOOL REPORT: [github] python-cyclonedx (scan duration: 4.2 seconds)
        requirements.txt components: 2 (License :: OSI Approved :: MIT License:1, License :: OSI Approved :: Apache Software License:1)
        requirements-dev.txt components: 3 (License :: OSI Approved :: MIT License:3)
        total: 6 (high:2, medium:3, low:1, warnings:true)
        ignored: 0 

        [HIGH DEPENDENCY] : pip (1.3.0)
        overview: The pip package before 19.2 for Python allows Directory Traversal when a URL is given in an install command, because a Content-Disposition header can have ../ in a filename, as demonstrated by overwriting the /root/.ssh/authorized_keys file. This occurs in _download_http_url in _internal/download.py.
        PYSEC: PYSEC-2020-173
        CVE: CVE-2019-20916
        recommendation: Update package to non-vulnerable version 19.2
        file: requirements.txt (line 1)

        [HIGH DEPENDENCY] : requests (2.4.0)
        overview: The Requests package before 2.20.0 for Python sends an HTTP Authorization header to an http URI upon receiving a same-hostname https-to-http redirect, which makes it easier for remote attackers to discover credentials by sniffing the network.
        PYSEC: PYSEC-2018-28
        CVE: CVE-2018-18074
        recommendation: Update package to non-vulnerable version 2.20.0
        file: requirements.txt (line 1)

        [MEDIUM DEPENDENCY] : pip (1.3.0)
        overview: A flaw was found in python-pip in the way it handled Unicode separators in git references. A remote attacker could possibly use this issue to install a different revision on a repository. The highest threat from this vulnerability is to data integrity. This is fixed in python-pip version 21.1.
        PYSEC: PYSEC-2021-437
        CVE: CVE-2021-3572
        recommendation: Update package to non-vulnerable version 21.1
        file: requirements.txt (line 1)

        [MEDIUM DEPENDENCY] : pip (1.3.0)
        overview: The mirroring support (-M, --use-mirrors) in Python Pip before 1.5 uses insecure DNS querying and authenticity checks which allows attackers to perform man-in-the-middle attacks.
        PYSEC: PYSEC-2019-160
        CVE: CVE-2013-5123
        recommendation: Update package to non-vulnerable version 1.5
        file: requirements.txt (line 1)

        [MEDIUM DEPENDENCY] : requests (2.4.0)
        overview: The resolve_redirects function in sessions.py in requests 2.1.0 through 2.5.3 allows remote attackers to conduct session fixation attacks via a cookie without a host value in a redirect.
        PYSEC: PYSEC-2015-17
        CVE: CVE-2015-2296
        recommendation: Update package to non-vulnerable version 2.6.0
        file: requirements.txt (line 1)

        [LOW DEPENDENCY] : pip (1.3.0)
        overview: pip 1.3 through 1.5.6 allows local users to cause a denial of service (prevention of package installation) by creating a /tmp/pip-build-* file for another user.
        PYSEC: PYSEC-2014-11
        CVE: CVE-2014-8991
        recommendation: Update package to non-vulnerable version 6.0
        file: requirements.txt (line 1)


    [trufflehog] Vulnerabilities
    =================================
    TOOL REPORT: [github] trufflehog (scan duration: 0.5 seconds)
        total: 45 (medium:40, low:5)
        ignored: 0 

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2153 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1217 characters)>
        file: eze.sarif (line 2153)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2123 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:                 "text": "'Consider possible security implications associated with the subprocess module.', in .\\insecure\\src\\super-insecure-\nlib.py Investigate '.\\insecure\\src\\super-insecure-lib.py' Line 1 for 'Consider possible security implications assoc\niated with the subprocess module.' strings Full Match: 1 import subprocess\n2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa \nAAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUw\nYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGF\nqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n"
        file: eze.sarif (line 2123)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2445 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\unpinned-requirements\\src\\super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EA\nAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1\nziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strin\ngs Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvyS\nmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuO\nL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@\nhackers.com\"\n"
        file: eze.sarif (line 2445)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2153 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1217 characters)>
        file: eze.sarif (line 2153)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2143 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1189 characters)>
        file: eze.sarif (line 2143)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2153 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1217 characters)>
        file: eze.sarif (line 2153)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2153 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1217 characters)>
        file: eze.sarif (line 2153)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2445 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\unpinned-requirements\\src\\super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EA\nAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1\nziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strin\ngs Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvyS\nmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuO\nL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@\nhackers.com\"\n"
        file: eze.sarif (line 2445)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2123 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:                 "text": "'Consider possible security implications associated with the subprocess module.', in .\\insecure\\src\\super-insecure-\nlib.py Investigate '.\\insecure\\src\\super-insecure-lib.py' Line 1 for 'Consider possible security implications assoc\niated with the subprocess module.' strings Full Match: 1 import subprocess\n2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa \nAAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUw\nYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGF\nqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n"
        file: eze.sarif (line 2123)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2425 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\insecure\\src\\super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp\n0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7\net/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match\n: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfar\nHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoP\ncxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.sarif (line 2425)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2425 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\insecure\\src\\super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp\n0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7\net/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match\n: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfar\nHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoP\ncxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.sarif (line 2425)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2133 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:                 "text": "'Consider possible security implications associated with the subprocess module.', in .\\unpinned-requirements\\src\\su\nper-insecure-lib.py Investigate '.\\unpinned-requirements\\src\\super-insecure-lib.py' Line 1 for 'Consider possible s\necurity implications associated with the subprocess module.' strings Full Match: 1 import subprocess\n2 \n3 INSECURE_\nSECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarH\njpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTu\nOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n"
        file: eze.sarif (line 2133)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2385 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\insecure\\src\\super-insecure-lib.py' Line 1 for 'Consider possible security implications associated with the subproc\ness module.' strings Full Match: 1 import subprocess\n2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG4\n2y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5G\nwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n"
        file: eze.sarif (line 2385)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2133 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:                 "text": "'Consider possible security implications associated with the subprocess module.', in .\\unpinned-requirements\\src\\su\nper-insecure-lib.py Investigate '.\\unpinned-requirements\\src\\super-insecure-lib.py' Line 1 for 'Consider possible s\necurity implications associated with the subprocess module.' strings Full Match: 1 import subprocess\n2 \n3 INSECURE_\nSECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarH\njpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTu\nOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n"
        file: eze.sarif (line 2133)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2143 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1189 characters)>
        file: eze.sarif (line 2143)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2405 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\unpinned-requirements\\src\\super-insecure-lib.py' Line 1 for 'Consider possible security implications associated wit\nh the subprocess module.' strings Full Match: 1 import subprocess\n2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAA\nAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x\n+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n"
        file: eze.sarif (line 2405)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2143 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1189 characters)>
        file: eze.sarif (line 2143)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2445 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\unpinned-requirements\\src\\super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EA\nAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1\nziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strin\ngs Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvyS\nmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuO\nL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@\nhackers.com\"\n"
        file: eze.sarif (line 2445)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2143 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1189 characters)>
        file: eze.sarif (line 2143)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2133 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:                 "text": "'Consider possible security implications associated with the subprocess module.', in .\\unpinned-requirements\\src\\su\nper-insecure-lib.py Investigate '.\\unpinned-requirements\\src\\super-insecure-lib.py' Line 1 for 'Consider possible s\necurity implications associated with the subprocess module.' strings Full Match: 1 import subprocess\n2 \n3 INSECURE_\nSECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarH\njpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTu\nOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n"
        file: eze.sarif (line 2133)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2425 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\insecure\\src\\super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp\n0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7\net/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match\n: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfar\nHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoP\ncxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.sarif (line 2425)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2405 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\unpinned-requirements\\src\\super-insecure-lib.py' Line 1 for 'Consider possible security implications associated wit\nh the subprocess module.' strings Full Match: 1 import subprocess\n2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAA\nAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x\n+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n"
        file: eze.sarif (line 2405)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2143 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1189 characters)>
        file: eze.sarif (line 2143)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2153 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1217 characters)>
        file: eze.sarif (line 2153)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2445 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\unpinned-requirements\\src\\super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EA\nAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1\nziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strin\ngs Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvyS\nmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuO\nL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@\nhackers.com\"\n"
        file: eze.sarif (line 2445)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2143 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1189 characters)>
        file: eze.sarif (line 2143)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2425 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\insecure\\src\\super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp\n0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7\net/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match\n: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfar\nHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoP\ncxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.sarif (line 2425)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2153 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1217 characters)>
        file: eze.sarif (line 2153)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2123 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:                 "text": "'Consider possible security implications associated with the subprocess module.', in .\\insecure\\src\\super-insecure-\nlib.py Investigate '.\\insecure\\src\\super-insecure-lib.py' Line 1 for 'Consider possible security implications assoc\niated with the subprocess module.' strings Full Match: 1 import subprocess\n2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa \nAAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUw\nYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGF\nqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n"
        file: eze.sarif (line 2123)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2148 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:               "name": "Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'",
        file: eze.sarif (line 2148)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2153 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1217 characters)>
        file: eze.sarif (line 2153)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2138 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:               "name": "Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'",
        file: eze.sarif (line 2138)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2143 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1189 characters)>
        file: eze.sarif (line 2143)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2143 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1189 characters)>
        file: eze.sarif (line 2143)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2153 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1217 characters)>
        file: eze.sarif (line 2153)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2425 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\insecure\\src\\super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp\n0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7\net/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match\n: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfar\nHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoP\ncxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.sarif (line 2425)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2153 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1217 characters)>
        file: eze.sarif (line 2153)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2445 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\unpinned-requirements\\src\\super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EA\nAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1\nziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strin\ngs Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvyS\nmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuO\nL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@\nhackers.com\"\n"
        file: eze.sarif (line 2445)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2385 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\insecure\\src\\super-insecure-lib.py' Line 1 for 'Consider possible security implications associated with the subproc\ness module.' strings Full Match: 1 import subprocess\n2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG4\n2y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5G\nwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n"
        file: eze.sarif (line 2385)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in src/super-insecure-lib.py
        recommendation: Investigate 'src/super-insecure-lib.py' Line 3 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: INSECURE_SECRET_RSA_KEY = "ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR"
        file: src/super-insecure-lib.py (line 3)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2425 for 'Password in URL' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\insecure\\src\\super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp\n0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7\net/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match\n: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfar\nHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoP\ncxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.sarif (line 2425)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2153 for 'Password in URL' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1217 characters)>
        file: eze.sarif (line 2153)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2445 for 'Password in URL' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate '.\\unpinned-requirements\\src\\super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EA\nAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1\nziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strin\ngs Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvyS\nmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuO\nL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@\nhackers.com\"\n"
        file: eze.sarif (line 2445)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 2143 for 'Password in URL' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1189 characters)>
        file: eze.sarif (line 2143)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in src/super-insecure-lib.py
        recommendation: Investigate 'src/super-insecure-lib.py' Line 5 for 'Password in URL' strings (add '# nosecret' to line if false positive) Full Match: INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = "https://admin:god@hackers.com"
        file: src/super-insecure-lib.py (line 5)


## Bill of Materials
---

![components](https://img.shields.io/static/v1?style=plastic&label=components&message=5&color=blue)

    ### [python-cyclonedx] requirements.txt SBOM
    ---

| type    | name     | version | license    | license type | description |
| ------- | -------- | ------- | ---------- | ------------ | ----------- |
| library | pip      | 1.3.0   | MIT        | permissive   |             |
| library | requests | 2.4.0   | Apache-2.0 | permissive   |             |

    ### [python-cyclonedx] requirements-dev.txt SBOM
    ---

| type    | name            | version | license | license type | description |
| ------- | --------------- | ------- | ------- | ------------ | ----------- |
| library | black           | 20.8b1  | MIT     | permissive   |             |
| library | pytest          | 6.2.2   | MIT     | permissive   |             |
| library | pytest-snapshot | 0.5.0   | MIT     | permissive   |             |

## Warnings
---

    [python-bandit] Warnings
    =================================
    {"filename": "app", "reason": "No such file or directory"}

    [python-safety] Warnings
    =================================
    Warning: unpinned requirement 'click' found in requirements.txt, unable to check.
    Warning: unpinned requirement 'click' found in requirements.txt, unable to check.
    

    [python-cyclonedx] Warnings
    =================================
    unable to check licenses, no valid license information in sboms
    unable to check licenses, no valid license information in sboms
    Warning: unpinned requirement 'click' found in requirements.txt, unable to check

