Version: NAFATH-V3
Track: Networking

## Overview
A government entity plans to introduce an AI chat assistant in its mobile application to help citizens find accurate information about public services. Software engineering supports reliable development, version control, and safe updates as the assistant evolves. Artificial intelligence helps interpret questions and retrieve relevant information from approved government resources. Mobile technology provides an accessible interface and protects communication between the application and its services. Networking connects users, servers, and information systems so requests and responses can travel reliably. Cybersecurity is essential to defend the assistant against malicious instructions and unauthorized access. Data management supports responsible handling of citizen information, including privacy and appropriate use of records. These six fields must work together to deliver a useful, trustworthy, and maintainable public service, with particular attention to IPv4 and IPv6 networking.

## Software
Semantic Versioning uses three numbers: MAJOR.MINOR.PATCH. A MAJOR version changes when an update breaks compatibility with existing users of an API. A MINOR version adds backward-compatible functionality, while a PATCH version fixes bugs without breaking compatibility. For the government's AI assistant, this approach helps developers communicate whether an API update introduces new features, corrects problems, or requires changes to the mobile application. It supports safer planning and coordination between development teams.

Resource: Semantic Versioning 2.0.0 – https://semver.org/spec/v2.0.0.html

## AI
Retrieval-Augmented Generation (RAG) combines an AI language model with information retrieved from external sources. For the government's AI chat assistant, RAG can retrieve relevant information from approved government documents before generating answers to citizens' questions. This helps keep responses grounded in official service information and reduces the risk of incorrect or outdated answers. However, RAG does not guarantee accuracy, so reliable sources, regular updates, and appropriate checks are still necessary.

Resource: IBM Research, What is retrieval-augmented generation (RAG)? – https://research.ibm.com/blog/retrieval-augmented-generation-RAG

## Mobile
Apple's App Transport Security (ATS) helps protect network connections made by iOS applications. By default, ATS requires secure HTTPS connections and restricts insecure HTTP traffic unless a specific exception is configured. For the government's mobile AI assistant, ATS helps protect communication when citizens send questions and receive answers. Developers should configure secure connections to government services and avoid unnecessary exceptions, reducing the risk of information being exposed during transmission.

Resource: Preventing Insecure Network Connections – https://developer.apple.com/documentation/security/preventing-insecure-network-connections

## Networking
IPv4 uses 32-bit addresses, while IPv6 uses 128-bit addresses, providing a much larger address space. For the government’s AI chat assistant, both protocols can support communication between citizens’ mobile devices and government servers. IPv6 also introduces differences in packet structure and addressing. However, using IPv6 does not automatically encrypt information. The project should support reliable connectivity and use appropriate security measures to protect citizens’ questions and responses during transmission.

Resource: RFC 8200, Internet Protocol, Version 6 (IPv6) Specification – https://www.rfc-editor.org/info/rfc8200/

## Cybersecurity
Prompt injection occurs when malicious instructions attempt to influence an AI assistant's behavior. Direct attacks come from users, while indirect attacks can appear in external documents or retrieved content. For the government's AI chat assistant, attackers might try to manipulate answers or expose sensitive information. Developers should treat retrieved content as untrusted, limit the assistant's permissions, and apply appropriate security checks to reduce these risks.

Resource: OWASP, LLM01: Prompt Injection – https://genai.owasp.org/llmrisk2023-24/llm01-24-prompt-injection/

## Data
Data anonymisation removes identifying information so individuals cannot be identified using reasonably likely means, while pseudonymisation replaces identifiers but may still allow re-identification using additional information. For the government's AI chat assistant, these techniques help protect citizens' privacy when handling questions, conversation records, and service data. Developers should minimise personal data collection, restrict access to sensitive records, and carefully assess whether information is truly anonymous before sharing or analysing it.

Resource: Introduction to Anonymisation – https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/data-sharing/anonymisation/introduction-to-anonymisation/
## Misconception in My Track
A common misconception is that IPv6 uses the same 32-bit address length as IPv4. In fact, IPv6 uses 128-bit addresses, providing a much larger address space. RFC 8200, Section 3 (IPv6 Header Format), identifies the Source Address and Destination Address fields as 128-bit addresses. This distinction matters for the government's AI chat assistant because its network infrastructure must support the correct addressing formats for both protocols. Developers should also remember that adopting IPv6 does not automatically encrypt communications. Appropriate security measures are still necessary to protect citizens' questions and responses.

## Open Question
How can the government ensure that its AI chat assistant remains accessible and secure for citizens using both IPv4 and IPv6 networks, especially when mobile network conditions vary?
