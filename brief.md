Version: NAFATH-V3

Your track: Networking

Overview
A trustworthy AI assistant in a government mobile app depends on six connected IT fields. Software engineering defines a stable public API so other services can use the assistant without unexpected changes. AI and retrieval-augmented generation (RAG) help produce answers grounded in reliable documents. Mobile security protects communication between the app and its services. Networking provides the addressing and connectivity needed to reach those services as more devices connect to the internet. Cybersecurity helps defend the assistant against threats such as prompt injection. Data practices determine how chat logs are protected and whether people can be identified. Together, these fields support a service that is useful, secure, and reliable for citizens. My Networking research focuses on IPv6 addressing and how it supports a growing number of connected devices.
Software
Semantic Versioning uses MAJOR, MINOR, and PATCH numbers to communicate the impact of API changes. A MAJOR version is required when an update introduces incompatible public API changes. A MINOR version is used when new functionality is added in a backward-compatible way. A PATCH version is used for backward-compatible bug fixes. For a government AI assistant, following these rules helps other systems know whether an update may require changes to their integrations.

Resource: Semantic Versioning 2.0.0
https://semver.org/spec/v2.0.0.html
AI
Retrieval-Augmented Generation (RAG) combines a language model with an information retrieval system. Instead of relying only on information learned during training, the assistant retrieves relevant material from trusted documents and uses it to help generate an answer. This can reduce incorrect answers by grounding responses in relevant sources, but it does not guarantee accuracy. The system should use reliable, updated documents and make uncertainty clear when evidence is missing.

Resource: What is Retrieval-Augmented Generation (RAG)?
https://cloud.google.com/use-cases/retrieval-augmented-generation
Mobile
Apple’s App Transport Security (ATS) requires network connections made through standard URL loading systems to meet security requirements, including secure HTTPS connections. It helps protect data in transit by restricting connections that do not meet these requirements. If an app attempts to connect to a plain HTTP endpoint, ATS will generally block the connection unless an exception has been configured. A government app should prefer HTTPS endpoints and avoid unnecessary security exceptions.

Resource: Preventing Insecure Network Connections
https://developer.apple.com/documentation/security/preventing-insecure-network-connections
Networking
IPv6 uses 128-bit addresses, while IPv4 uses 32-bit addresses. This creates a much larger address space in IPv6, allowing far more unique addresses for internet-connected devices. As governments connect more mobile apps, sensors, and online services, the availability of addresses becomes increasingly important. IPv6 also includes features designed to support modern internet communication. Planning for IPv6 helps public services accommodate growth without depending only on the limited IPv4 address space.

Resource: RFC 8200 — Internet Protocol, Version 6 (IPv6) Specification
https://www.rfc-editor.org/info/rfc8200/
Cybersecurity
Prompt injection is an attack in which someone uses input to manipulate an AI system into ignoring its intended instructions. Direct prompt injection comes from content entered by a user, while indirect prompt injection is hidden in external content, such as a webpage or document, that the AI retrieves or processes. Risk-reduction methods include treating retrieved content as untrusted data and limiting the assistant’s permissions. Testing with adversarial examples and keeping human oversight for sensitive actions can also reduce risk.

Resource: LLM01: Prompt Injection
https://genai.owasp.org/llmrisk2023-24/llm01-24-prompt-injection/
Data
Anonymization and pseudonymization are different ways to reduce privacy risks in chat logs. Anonymization aims to prevent people from being identified, while pseudonymization replaces identifying details with codes or other identifiers that may still be linked back to a person using additional information. Under UK data protection law, genuinely anonymous information falls outside the scope of personal data protection rules, but pseudonymized data generally remains personal data. A government assistant should minimize collected data and assess whether re-identification is possible.

Resource: Introduction to Anonymisation
https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/data-sharing/anonymisation/introduction-to-anonymisation/
Misconception in My Track
A common misconception is that IPv6 is simply a longer version of IPv4 and that its only benefit is providing more addresses. In fact, IPv6 is a distinct Internet Protocol version with its own packet format and addressing architecture. Its 128-bit addresses provide a vastly larger address space than IPv4’s 32-bit addresses, helping support the growth of connected devices. RFC 8200, in the section titled “Introduction,” describes IPv6 as the successor to IPv4 and explains its basic design. This shows that IPv6 is an important protocol evolution, not just a longer address.

Resource evidence: RFC 8200, “Introduction”
https://www.rfc-editor.org/rfc/rfc8200.html#section-1
Open Question
How can a government mobile service introduce IPv6 while continuing to support citizens and systems that still rely on IPv4?
