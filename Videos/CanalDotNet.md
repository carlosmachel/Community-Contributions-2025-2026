# Youtube

<b>Number of contributions: 15</b>

<table>
  <tr>
    <td align=center><b>Number</b></td>
    <td align=center><b>Date</b></td>
    <td align=center><b>Title</b></td>
    <td align=center><b>Description</b></td>
    <td align=center><b>Link</b></td>
    <td align=center><b>Link Linkedin</b></td>
  </tr>  
  <tr>
  <td align=center>1</td>
      <td align=center>June 18, 2025</td>
      <td align=center>Artificial Intelligence Fundamentals: Agents, Assistants, Bots, Observability…</td>
      <td align=center>In this live session, the topics covered focused on the definition and operation of AI agents, highlighting autonomy as the main differentiator between bots, assistants, and agents. While assistants merely help users, agents are capable of completing objectives independently, using a structure composed of instructions, language models, and tools. The integration of these components in Azure AI Foundry and the use of Semantic Kernel for code-level orchestration were discussed.
A key topic was observability, with OpenTelemetry identified as the standard for tracking token consumption and agent execution logic on platforms like Grafana and Application Insights. Through practical examples, such as the "Contoso Açaí" project, the experts demonstrated how agents solve real business problems by natively accessing databases and APIs. Finally, the constant evolution of SDKs and the critical importance of conversation tracing for debugging in production environments were emphasized.</td>
      <td align=center><a href="https://www.youtube.com/watch?v=f1QGl5Z_Jws">Link</a></td>
      <td align=center></td>
  </tr>
  <tr>
      <td align=center>2</td>
      <td align=center>June 24, 2025</td>
      <td align=center>Artificial Intelligence Fundamentals: Model Context Protocol (MCP) – What It Is and Its Benefits</td>
      <td align=center>This live session presents the Model Context Protocol (MCP) as an open standard that functions as a USB port for Artificial Intelligence, standardizing the connection of data peripherals and tools to language models. The ecosystem demonstrates maturity with SDK support in C#, Python, TypeScript, Java, Swift, and Kotlin. Its architecture decouples information sources through Host, Client, and Server, where the server acts as a bridge exposing local or remote capabilities via standardized interfaces. The session also addresses current security weaknesses, such as prompt injection risks, emphasizing the importance of ensuring that permissions are not bypassed and restricting agents to predefined and authorized actions to prevent malicious commands. Finally, it explores Azure AI Foundry Local, which enables model execution via ONNX Runtime on Windows and Mac. The tool removes Development complexity by automatically identifying and optimizing the use of CPU, GPU, or NPU, enabling robust and cloud-independent solutions.</td>
      <td align=center><a href="https://www.youtube.com/watch?v=0Gxq9ITeUBw">Link</a></td>
      <td align=center></td>
  </tr>
  <tr>
      <td align=center>3</td>
      <td align=center>July 10, 2025</td>
      <td align=center>Artificial Intelligence Fundamentals: A2A – Agent-to-Agent – An Overview of the Protocol</td>
      <td align=center>This video discusses innovations and challenges in the field of Artificial Intelligence, with a central focus on the A2A (Agent-to-Agent) protocol.
The main points covered are:
A2A Protocol vs. MCP: The video explains that A2A, created by Google and adopted by Microsoft, is a protocol specifically designed for communication between agents, including connections with agents outside closed ecosystems. MCP, on the other hand, is aimed at integration between agents and tools.
Experimental Status: It emphasizes that both A2A and MCP are still in experimental stages, with documentation and architecture diagrams in the maturation phase.
Security and Risks: The video discusses the major technical challenges, especially the vulnerability to prompt injection. It warns that agents without proper filters or permissions can be induced to execute malicious commands, such as SQL instructions to drop databases.
Platform Evolution: It mentions how Microsoft AI Foundry is becoming an "umbrella" for grouping various generative AI services.
Practical Applications: The video notes that the use of agents for support in code structures and business architecture already shows interesting results, being considered a point of no return for the industry.</td>
      <td align=center><a href="https://www.youtube.com/watch?v=5wo_YJk8_8Q">Link</a></td>
      <td align=center></td>
  </tr>
   <tr>
      <td align=center>4</td>
      <td align=center>August 21, 2025</td>
      <td align=center>Best Practices in Artificial Intelligence: Security Tips and Recommendations with MCP Servers</td>
      <td align=center>
      This video addresses security best practices for MCP (Model Context Protocol), described as a "USB" that connects AI models to various tools and repositories. The experts warn about the risks of using unofficial MCPs, which can capture sensitive data such as Personal Access Tokens (PATs). A critical point discussed is excessive permissions; it is recommended to apply the Zero Trust concept, limiting access to "read-only" to mitigate damage caused by AI hallucinations or prompt injection attacks.
The lack of native authentication in many servers requires external protections, such as using API Management or Microsoft Entra ID. Additionally, observability through OpenTelemetry is essential for tracking agent actions and detecting malicious behavior in real-time. Finally, the need for caution with the "supply chain" and conducting tests in controlled environments before production is emphasized.
</td>
      <td align=center><a href="https://www.youtube.com/watch?v=U7TNxzI07C4">Link</a></td>
      <td align=center><a href="">Link</a></td>
  </tr>  
  <tr>
      <td align=center>5</td>
      <td align=center>August 27, 2025</td>
      <td align=center>Artificial Intelligence Security: Main Attacks Using MCP Servers and How to Avoid Them!</td>
      <td align=center>
      This video addresses security risks and best practices when using Model Context Protocol (MCP) servers in AI agents. Among the main attacks discussed are "poison tool description," where malicious descriptions deceive AI into executing improper actions (such as leaking private conversations), and "name collision," which uses names similar to legitimate tools to mislead the system. Another highlighted danger is the "cross-connector" attack, where a hidden command in a document triggers malicious actions through another connector.
To mitigate these threats, experts recommend the principle of least privilege, limiting tool permissions to what is strictly necessary. It is suggested to prioritize verified sources, such as the Docker catalog, or develop custom MCPs to maintain full control over data and credentials. Finally, the use of automated filters, template sanitization, and observability tools (tracing) are essential for monitoring suspicious interactions.
</td>
      <td align=center><a href="https://www.youtube.com/watch?v=tuLGlpRKPXQ">Link</a></td>
      <td align=center></td>
  </tr>
  <tr>
      <td align=center>6</td>
      <td align=center>September 4, 2025</td>
      <td align=center>What You Need to Know About Prompt Injection</td>
      <td align=center>
      This video provides a technical and practical approach to Prompt Injection, identified as the number one vulnerability in the OWASP Top 10 list for LLMs. The experts demonstrate how to bypass AI security restrictions through context techniques, such as using "movie scripts" to force prohibited translations or extracting system prompts and internal tools. Advanced attacks using special tokens (such as <|im_start|>) and the "Crescendo" method, which automates manipulation through gradual dialogues, are discussed.
A critical highlight is database integration, where prompt injection can trigger SQL Injection, allowing destructive commands like DROP TABLE even against explicit security instructions. For mitigation, the speakers emphasize the Principle of Least Privilege, limiting AI access permissions, and the use of Guardrails and tools like Azure AI Content Safety. The conclusion is that relying solely on text instructions is dangerous, making it essential to technically validate all inputs and outputs.
      </td>
      <td align=center><a href="https://www.youtube.com/watch?v=JUqSO07-xRk">Link</a></td>
      <td align=center></td>
  </tr>
  <tr>
      <td align=center>7</td>
      <td align=center>September 19, 2025</td>
      <td align=center>Roundtable #233: Open Source from A to Z – Projects, Tips, Possibilities… | 19th Edition</td>
      <td align=center>
      The video "Roundtable #233" addresses security in the open source ecosystem and supply chain attacks. Participants discuss recent incidents, such as the credential leak at CrowdStrike via infected npm packages and a critical vulnerability in Microsoft Entra ID that allowed administrative access between different tenants through JWT tokens. They highlight how Artificial Intelligence is being used to bypass security systems, including Captcha and facial biometrics bypass.
The live session explores educational resources from API Security University and focuses on items from the OWASP Top 10 list for Open Source Software, detailing known vulnerabilities (CVEs) and the compromise of legitimate packages. Tools like GitHub Dependabot, Snyk, and Checkmarx are recommended for risk mitigation. Finally, the experts debate the impact of post-quantum computing on cryptography and recall technological evolution, from the era of floppy disks to modern Docker images.
</td>
      <td align=center><a href="https://www.youtube.com/watch?v=Hd2kmAYUZ1k">Link</a></td>
      <td align=center></td>
  </tr>
  <tr>
      <td align=center>8</td>
      <td align=center>November 27, 2025</td>
      <td align=center>OWASP Top 10 Risks for Open Source Software + Vulnerabilities in Application Dependencies</td>
      <td align=center>
      This video covers the OWASP Top 10 list specifically focused on open source software, highlighting security risks in dependencies and packages such as npm, NuGet, Maven, and Docker images. The speakers discuss the first item on the list, "Known Vulnerabilities," emphasizing the importance of monitoring CVEs and using databases like NIST and GitHub Security Advisories.
A critical point detailed is the concept of transitive dependencies, exemplified by the global impact of the Log4j vulnerability, which affected the integrity and availability of large-scale systems. Additionally, the video warns about the risk of "Name Confusion," where malicious packages imitate legitimate names to deceive developers.
For mitigation, it is recommended to use GitHub Dependabot, which automates security alerts. Finally, analysis tools such as Snyk, Checkmarx, and open source options like OWASP Dependency Check and Docker Scout are presented.
</td>
      <td align=center><a href="https://www.youtube.com/watch?v=3ClYzPiCuEY">Link</a></td>
      <td align=center></td>
  </tr>
   <tr>
      <td align=center>9</td>
      <td align=center>December 3, 2025</td>
      <td align=center>OWASP Top 10 Risks for Open Source Software: Packages and Dependencies with Compromised Security</td>
      <td align=center>
      This video addresses the risks listed in the OWASP Top 10 for Open Source Software (OSS), with special focus on the compromise of legitimate packages. The experts discuss how attackers inject malicious code into trusted projects through maintainer account hijacking or repository vulnerabilities, affecting build system integrity and data.
Real cases of supply chain attacks are analyzed, such as SolarWinds and the misuse of pipelines for Bitcoin mining. The debate also details injection vulnerabilities (SQL, system commands, and APIs), noting that the npm ecosystem is particularly targeted due to automatic version update practices.
As mitigation measures, the video recommends using secure internal repositories (such as Nexus or Harbor) for dependency caching, code reviews, and adopting security frameworks to verify component provenance.
</td>
      <td align=center><a href="https://www.youtube.com/watch?v=cScCo1rBdKk">Link</a></td>
      <td align=center></td>
  </tr>
<tr>
      <td align=center>10</td>
      <td align=center>December 12, 2025</td>
      <td align=center>Microsoft Ignite 2025: Key Announcements – Azure, AI, Data, and Much More!</td>
      <td align=center>
      This video details the main announcements from Microsoft Ignite 2025, with an intense focus on Artificial Intelligence. One highlight is Microsoft AI Foundry, which unifies tools like the Agent Framework and offers Model Router for cost and performance optimization. The evolution of Copilot Studio is discussed, allowing the creation of low-code agents integrated with Teams and Microsoft 365, enhanced by "Work IQ" for personalized learning based on daily user activity.
The broadcast also covers the Model Context Protocol (MCP), highlighting its rapid adoption by tech giants and the recent donation of the protocol to the Linux Foundation. The experts explore agent security through the OWASP report and present practical demonstrations using Docker Desktop and VS Code to connect models to external tools. Finally, the Copilot Migration Agent is presented, designed to automate and facilitate migration of on-premises infrastructure to the Azure cloud.
      </td>
      <td align=center><a href="https://www.youtube.com/watch?v=biif288dofg">Link</a></td>
      <td align=center></td>
  </tr>
  <tr>
      <td align=center>11</td>
      <td align=center>December 17, 2025</td>
      <td align=center>What’s New in MCP + AI: Free Certification, Linux Foundation, Agentic AI Foundation…</td>
      <td align=center>
      This video details the main updates on the Model Context Protocol (MCP), highlighting its rapid rise as an essential open standard for the Agentic AI era. The key milestone is the donation of the protocol by Anthropic to the Linux Foundation, where it will be managed by the newly created Agentic AI Foundation, alongside other protocols such as A2A and ACP. This transition ensures neutral and stable governance, following the successful model of the Kubernetes ecosystem.
The content explores the support from tech giants like Microsoft, GitHub, and Google, while discussing the technical evolution of MCP, which now enables secure remote executions and greater interoperability between platforms. The experts also recommend a free certification offered by API SEC University for those who want to dive deeper into the topic. With over 700,000 repositories on GitHub, MCP is establishing itself as a vital infrastructure for connecting LLMs to complex systems.
      </td>
      <td align=center><a href="https://www.youtube.com/watch?v=uvCbxLpbTNo">Link</a></td>
      <td align=center></td>
  </tr>
    <tr>
      <td align=center>12</td>
      <td align=center>December 23, 2025</td>
      <td align=center>OWASP MCP Top 10: Security in Integrations with Artificial Intelligence</td>
      <td align=center>
      This video addresses the main security vulnerabilities in using the Model Context Protocol (MCP), a protocol widely adopted in AI integrations. The experts highlight ten critical risks: token and secrets exposure, privilege escalation via excessive scopes, tool poisoning with malicious instructions, software supply chain attacks, malicious command and prompt injection, authentication and authorization failures, lack of auditing and telemetry, use of unapproved MCP servers (shadow MCPs), and information leakage via context injection.
As best practices, they recommend consuming MCPs from trusted sources like the Docker MCP Catalog, protecting integrations with API Gateways and identity providers like Microsoft Entra, adopting OpenTelemetry for monitoring, and always applying the principle of least privilege to AI agents.
</td>
      <td align=center><a href="https://www.youtube.com/watch?v=HUuAs9R9Hag">Link</a></td>
      <td align=center><a href="https://www.linkedin.com/posts/carlosmachel_online-1330-owasp-mcp-top-10-ia-activity-7409236185669263360-3pUD?utm_source=share&utm_medium=member_desktop&rcm=ACoAABwDPuMBUIynDxpLtAB9N7-XCR_m6IhWMLg">Link</a></td>
  </tr>
  <tr>
      <td align=center>13</td>
      <td align=center>March 5, 2026</td>
      <td align=center>Code Security: some considerations, best practices, support tools...</td>
      <td align=center>Check out this video for a discussion on how to implement more secure code in application development: Well-Architected Framework, issues involving data privacy, Artificial Intelligence, recommendations that integrate the OWASP Cheat Sheet Series, SAST (Static Application Security Testing), DAST (Dynamic Application Security Testing), Grafana dashboards for security analysis in containers/Kubernetes, open source tools...</td>
      <td align=center><a href="https://www.youtube.com/watch?v=Kk_aKMR65mE">Link</a></td>
      <td align=center><a href="">Link</a></td>
  </tr>
    <tr>
      <td align=center>14</td>
      <td align=center>March 6, 2026</td>
      <td align=center>Arquiteturas de Referência em Inteligência Artificial: uma visão geral do Microsoft Learn MCP Server</td>
      <td align=center>Confira neste vídeo uma discussão sobre como o MCP Server do Microsoft Learn foi implementado: a escolha por uma aplicação que implementa o protocolo MCP ao invés de uma API REST convencional, o uso combinado de serviços como Azure App Service, Azure Blob Storage e Azure AI Search, quais fatores foram levados em consideração ao expor publicando um MCP Server na nuvem e muito mais!</td>
      <td align=center><a href="https://www.youtube.com/watch?v=-8ow0yJfils">Link</a></td>
      <td align=center><a href="https://www.linkedin.com/posts/carlosmachel_ai-mcp-modelcontextprotocol-activity-7435805853699571712-7WP9?utm_source=share&utm_medium=member_desktop&rcm=ACoAABwDPuMBUIynDxpLtAB9N7-XCR_m6IhWMLg">Link</a></td>
  </tr>

<tr>
      <td align=center>15</td>
      <td align=center>March 10, 2026</td>
      <td align=center>Certificações Microsoft: novos exames e grandes mudanças para o ano de 2026!</td>
      <td align=center>Confira neste evento ONLINE e GRATUITO do Canal .NET e do Coding Night uma série de mudanças previstas para exames de certificação da Microsoft: novos exames, certificações que serão aposentadas, o que estudar diante de um foco maior em soluções de Inteligência Artificial e muito mais!
</td>
      <td align=center><a href="https://www.youtube.com/watch?v=3kFud3sSxCU">Link</a></td>
      <td align=center><a href="https://www.linkedin.com/posts/carlosmachel_ai-microsoft-certifications-activity-7437485877867642880-tzGY?utm_source=share&utm_medium=member_desktop&rcm=ACoAABwDPuMBUIynDxpLtAB9N7-XCR_m6IhWMLg">Link</a></td>
  </tr>
  </table>