Version: NAFATH-V3

Your track: Networking

Overview
A trustworthy AI assistant in a government mobile app depends on six connected IT fields. Software engineering defines a stable public API so other services can use the assistant without unexpected changes. AI and retrieval-augmented generation (RAG) help produce answers grounded in reliable documents. Mobile security protects communication between the app and its services. Networking provides the addressing and connectivity needed to reach those services as more devices connect to the internet. Cybersecurity helps defend the assistant against threats such as prompt injection. Data practices determine how chat logs are protected and whether people can be identified. Together, these fields support a service that is useful, secure, and reliable for citizens. For my Networking track, I will examine how IPv6 addressing supports a growing number of connected devices.
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

Cybersecurity

Data

Misconception in My Track

Open Question
