Version: NAFATH-V4

Track: Cybersecurity

## Overview
Software supply chain security protects the software, AI models, mobile applications, network routes, and data that a national service provider depends on. These components are connected, so a weakness in one area can affect the entire service. Software configuration and secret management help prevent credentials from being exposed in source code. AI security addresses attacks that manipulate training data or model behavior. Mobile application security standards provide a structured way to verify that applications meet security requirements. Network security helps detect and prevent unauthorized internet route changes, while Resource Public Key Infrastructure (RPKI) helps validate route origin information. Cybersecurity practices, including identifying and patching vulnerabilities such as Log4Shell, reduce the risk of exploitation. Finally, a Software Bill of Materials (SBOM) records software components and supports vulnerability tracking. Together, these six fields help teams assess dependencies, reduce risks, respond to threats, and maintain the integrity and availability of essential national services.

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

## Cybersecurity

## Data

## Misconception in My Track

## Open Question
