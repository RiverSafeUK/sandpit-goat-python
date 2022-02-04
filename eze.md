  
# Eze Report Results


## Summary  ![tools](https://img.shields.io/static/v1?style=plastic&label=Tools&message=5&color=blue)
---


![critical](https://img.shields.io/static/v1?style=plastic&label=critical&message=0&color=red)
![high](https://img.shields.io/static/v1?style=plastic&label=high&message=3&color=orange)
![medium](https://img.shields.io/static/v1?style=plastic&label=medium&message=29&color=yellow)
![low](https://img.shields.io/static/v1?style=plastic&label=low&message=10&color=lightgrey)
            
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
    TOOL REPORT: [github] python-piprot (scan duration: 0.2 seconds)
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
    TOOL REPORT: [github] python-safety (scan duration: 3.2 seconds)
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
        overview: Pip 21.1 updates its dependency 'urllib3' to v1.26.4 due to security issues.
        recommendation: Update pip (1.3.0) to a non vulnerable version, vulnerable versions: <21.1

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
    TOOL REPORT: [github] python-cyclonedx (scan duration: 5.1 seconds)
        requirements.txt components: 2 (License :: OSI Approved :: MIT License:1, License :: OSI Approved :: Apache Software License:1)
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
    TOOL REPORT: [github] trufflehog (scan duration: 0.4 seconds)
        total: 32 (medium:23, low:9)
        ignored: 0 

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 181 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.sarif' Line 1385 for 'High Entropy' strings Full Match:             "text": "Investigate './src/super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.md (line 181)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 181 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.sarif' Line 1385 for 'High Entropy' strings Full Match:             "text": "Investigate './src/super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.md (line 181)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 216 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.sarif' Line 1158 for 'High Entropy' strings Full Match:               "name": "Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'",
        file: eze.md (line 216)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 176 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.sarif' Line 1385 for 'High Entropy' strings Full Match:             "text": "Investigate './src/super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.md (line 176)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 176 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.sarif' Line 1385 for 'High Entropy' strings Full Match:             "text": "Investigate './src/super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.md (line 176)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 211 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.sarif' Line 1160 for 'High Entropy' strings Full Match:                 "text": "'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'', in ./src/super-insecure-lib.py"
        file: eze.md (line 211)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 186 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.sarif' Line 1153 for 'High Entropy' strings Full Match:                 "text": "'Consider possible security implications associated with the subprocess module.', in ./src/super-insecure-lib.py. Investigate './src/super-insecure-lib.py' Line 1 for 'Consider possible security implications associated with the subprocess module.' strings Full Match: 1 import subprocess\n2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n"
        file: eze.md (line 186)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 171 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.md' Line 148 for 'High Entropy' strings Full Match:         recommendation: Investigate 'eze.md' Line 148 for 'High Entropy' strings Full Match:         recommendation: Investigate 'src/super-insecure-lib.py' Line 3 for 'High Entropy' strings Full Match: INSECURE_SECRET_RSA_KEY = "ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR"
        file: eze.md (line 171)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 206 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.sarif' Line 1365 for 'High Entropy' strings Full Match:             "text": "Investigate './src/super-insecure-lib.py' Line 1 for 'Consider possible security implications associated with the subprocess module.' strings Full Match: 1 import subprocess\n2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n"
        file: eze.md (line 206)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 241 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.sarif' Line 1385 for 'Password in URL' strings Full Match:             "text": "Investigate './src/super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.md (line 241)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 241 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.sarif' Line 1385 for 'Password in URL' strings Full Match:             "text": "Investigate './src/super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.md (line 241)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 221 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'src/super-insecure-lib.py' Line 3 for 'High Entropy' strings Full Match: INSECURE_SECRET_RSA_KEY = "ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR"
        file: eze.md (line 221)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 166 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.md' Line 153 for 'High Entropy' strings Full Match:         recommendation: Investigate 'src/super-insecure-lib.py' Line 3 for 'High Entropy' strings Full Match: INSECURE_SECRET_RSA_KEY = "ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR"
        file: eze.md (line 166)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 1163 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1148 characters)>
        file: eze.sarif (line 1163)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 1163 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1148 characters)>
        file: eze.sarif (line 1163)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 1163 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1148 characters)>
        file: eze.sarif (line 1163)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 1153 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:                 "text": "'Consider possible security implications associated with the subprocess module.', in ./src/super-insecure-lib.py. Investigate './src/super-insecure-lib.py' Line 1 for 'Consider possible security implications associated with the subprocess module.' strings Full Match: 1 import subprocess\n2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n"
        file: eze.sarif (line 1153)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 1365 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate './src/super-insecure-lib.py' Line 1 for 'Consider possible security implications associated with the subprocess module.' strings Full Match: 1 import subprocess\n2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n"
        file: eze.sarif (line 1365)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 1158 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:               "name": "Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'",
        file: eze.sarif (line 1158)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 1385 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate './src/super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.sarif (line 1385)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 1385 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate './src/super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.sarif (line 1385)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 1160 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match:                 "text": "'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'', in ./src/super-insecure-lib.py"
        file: eze.sarif (line 1160)

        [MEDIUM SECRET] : Found Hardcoded 'High Entropy' Pattern
        overview: Found Hardcoded 'High Entropy' Pattern in src/super-insecure-lib.py
        recommendation: Investigate 'src/super-insecure-lib.py' Line 3 for 'High Entropy' strings (add '# nosecret' to line if false positive) Full Match: INSECURE_SECRET_RSA_KEY = "ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR"
        file: src/super-insecure-lib.py (line 3)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 226 for 'Password in URL' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.md' Line 158 for 'Password in URL' strings Full Match:         recommendation: Investigate 'eze.md' Line 153 for 'Password in URL' strings Full Match:         recommendation: Investigate 'src/super-insecure-lib.py' Line 5 for 'Password in URL' strings Full Match: INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = "https://admin:god@hackers.com"
        file: eze.md (line 226)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 231 for 'Password in URL' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.md' Line 163 for 'Password in URL' strings Full Match:         recommendation: Investigate 'src/super-insecure-lib.py' Line 5 for 'Password in URL' strings Full Match: INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = "https://admin:god@hackers.com"
        file: eze.md (line 231)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 181 for 'Password in URL' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.sarif' Line 1385 for 'High Entropy' strings Full Match:             "text": "Investigate './src/super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.md (line 181)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 241 for 'Password in URL' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.sarif' Line 1385 for 'Password in URL' strings Full Match:             "text": "Investigate './src/super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.md (line 241)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 176 for 'Password in URL' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'eze.sarif' Line 1385 for 'High Entropy' strings Full Match:             "text": "Investigate './src/super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.md (line 176)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in eze.md
        recommendation: Investigate 'eze.md' Line 246 for 'Password in URL' strings (add '# nosecret' to line if false positive) Full Match:         recommendation: Investigate 'src/super-insecure-lib.py' Line 5 for 'Password in URL' strings Full Match: INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = "https://admin:god@hackers.com"
        file: eze.md (line 246)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 1385 for 'Password in URL' strings (add '# nosecret' to line if false positive) Full Match:             "text": "Investigate './src/super-insecure-lib.py' Line 3 for 'Possible hardcoded password: 'ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR'' strings Full Match: 2 \n3 INSECURE_SECRET_RSA_KEY = \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAp0A7aEqG42y0q22yU+dLFMrlVhnk2C94QChUwZv0pKmEvySmzSGSY2gSMfarHjpKcW8OKZ5bcmgkZZ3sRkLJSUwYui/pZxOkUIKZ/sUsFDrW4souGPLfP1ziX/Rj0x+MXj7et/cKO5GwqanXrULssdXapaTz4W+OmMkSpPjtDC2lbfTuOL7lYE1cfbluoPcxvU2kw0ZIGFqOCFar2It33Xsie1C+//qIX3QWjJAvYF0ZF+OR\"\n4 \n5 INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = \"https://admin:god@hackers.com\"\n"
        file: eze.sarif (line 1385)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in eze.sarif
        recommendation: Investigate 'eze.sarif' Line 1163 for 'Password in URL' strings (add '# nosecret' to line if false positive) Full Match: <on long line (1148 characters)>
        file: eze.sarif (line 1163)

        [LOW SECRET] : Found Hardcoded 'Password in URL' Pattern
        overview: Found Hardcoded 'Password in URL' Pattern in src/super-insecure-lib.py
        recommendation: Investigate 'src/super-insecure-lib.py' Line 5 for 'Password in URL' strings (add '# nosecret' to line if false positive) Full Match: INSECURE_URL_WITH_HARDCODED_BASIC_AUTH = "https://admin:god@hackers.com"
        file: src/super-insecure-lib.py (line 5)


## Bill of Materials
---

![components](https://img.shields.io/static/v1?style=plastic&label=components&message=2&color=blue)

    ### [python-cyclonedx] requirements.txt SBOM
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

