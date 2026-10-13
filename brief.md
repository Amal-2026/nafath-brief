Version: NAFATH-V4

Track: Cybersecurity

## Overview
## Overview
Software supply chain security protects the software, AI models, mobile applications, network routes, and data used by a national service provider. Since these components are connected, a weakness in one can affect the entire service. Secure configuration and secret management prevent credentials from being exposed in source code. AI security addresses attacks that manipulate training data or model behavior, while mobile security standards help verify application protections. Network security and Resource Public Key Infrastructure (RPKI) help detect unauthorized routing changes and validate route origins. Cybersecurity practices reduce exploitation risks by identifying and patching vulnerabilities. A Software Bill of Materials (SBOM) records software components and supports vulnerability tracking. Together, these fields help teams manage dependencies, reduce risks, and maintain essential services. For the cybersecurity track, understanding and mitigating vulnerabilities such as Log4Shell is essential to protecting national services.

## Software
The Twelve-Factor App methodology states that configuration should be stored in environment variables, separate from application code. This includes database credentials, API keys, and service addresses that may change between deployments. Keeping secrets out of code reduces the risk of exposing them through public repositories, code reviews, or shared files. Sensitive values should be managed securely, with restricted access and appropriate secret-management tools.

Resource: The Twelve-Factor App – Config - https://12factor.net/config

## AI
Adversarial attacks target machine learning systems to cause incorrect outputs, expose information, or misuse model capabilities. Evasion attacks modify inputs during operation so that a model makes wrong predictions, while poisoning attacks manipulate training data to influence what the model learns. Privacy attacks attempt to reveal sensitive information about training data or model behavior. These attacks occur at different stages of the AI lifecycle and require testing, data protection, monitoring, and appropriate mitigation measures.

Resource: NIST – Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations - https://csrc.nist.gov/pubs/ai/100/2/e2025/final

## Mobile
The OWASP Mobile Application Security Verification Standard (MASVS) defines security controls for assessing mobile applications on platforms such as Android and iOS. It covers secure storage, cryptography, authentication, network communication, platform interaction, code quality, resilience, and privacy. Developers and security testers use these controls as a baseline to assess an app and identify weaknesses. The OWASP Mobile Application Security Testing Guide (MASTG) provides testing guidance to help verify whether the controls are implemented correctly.

Resource: OWASP – Mobile Application Security Verification Standard (MASVS) - https://mas.owasp.org/MASVS/

## Networking
Border Gateway Protocol (BGP) allows networks to exchange internet routing information. In a route hijacking attack, an attacker announces false routing information, potentially diverting traffic to an unauthorized network. Resource Public Key Infrastructure (RPKI) helps routers verify whether an autonomous system is authorized to originate an IP prefix. However, origin validation does not verify the entire route path or prevent every interception attack. Networks should also use routing policies, monitoring, and additional security measures.

Resource: RFC 6811 – BGP Prefix Origin Validation - https://www.rfc-editor.org/rfc/rfc6811.html
## Cybersecurity
Log4Shell (CVE-2021-44228) was a critical remote code execution vulnerability in the Apache Log4j Java logging library. An attacker could exploit vulnerable systems by sending specially crafted input that triggered unsafe lookups, potentially allowing code execution on the server. It was rated severe because exploitation could be relatively easy and lead to major compromise. Organizations should identify affected systems and upgrade to a fixed Log4j version, following official vendor guidance.

Resource: CISA – Mitigating Log4Shell and Other Log4j-Related Vulnerabilities - https://www.cisa.gov/news-events/cybersecurity-advisories/aa21-356a

## Data
A Software Bill of Materials (SBOM) is a structured inventory of software components and their relationships. It helps organizations identify dependencies and assess whether their software contains vulnerable or outdated components. The NTIA identifies minimum data fields including supplier name, component name, component version, other unique identifiers, dependency relationships, SBOM author, and timestamp. Maintaining an accurate SBOM improves transparency and supports vulnerability management across the software supply chain.

Resource: NTIA – The Minimum Elements for a Software Bill of Materials (SBOM) - https://www.ntia.gov/report/2021/minimum-elements-software-bill-materials-sbom

## Misconception in My Track
A common misconception is that Log4Shell only affects websites that use Java directly or that installing a firewall is enough to protect against it. In reality, the vulnerability affects vulnerable versions of the Apache Log4j logging library, which may be included indirectly through application dependencies. Attackers may exploit affected systems to execute code remotely. The correct response is to identify vulnerable Log4j versions, update to a fixed version, and follow vendor guidance. CISA's Log4Shell advisory explains the vulnerability and recommends mitigation actions.

Evidence: CISA – Mitigating Log4Shell and Other Log4j-Related Vulnerabilities, section “Mitigations”.
Supporting sentence: “Immediately identify, mitigate, and update affected products that use Log4j to the latest patched version.”

## Open Question
How can a national service provider continuously verify the integrity of software dependencies and detect newly disclosed vulnerabilities before attackers exploit them?
