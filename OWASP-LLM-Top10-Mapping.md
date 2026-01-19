# OWASP LLM Top 10 Vulnerabilities Checklist & Mapping (2025/2026)

**Purpose**: Identify, assess, and mitigate top risks in Large Language Model applications.  
**Source**: OWASP Top 10 for LLM Applications v1.1 / 2025 updates  
**License**: MIT – Free to use

## LLM01: Prompt Injection
- [ ] Use privilege control / prompt isolation
- [ ] Enforce strict input validation & sanitization
- [ ] Implement output filtering & privilege boundaries
- [ ] Use separate LLM for guardrails

## LLM02: Insecure Output Handling
- [ ] Validate & sanitize all LLM outputs before use
- [ ] Avoid direct rendering of LLM content in privileged contexts
- [ ] Apply least-privilege principle to downstream systems

## LLM03: Training Data Poisoning
- [ ] Vet external data sources & training sets
- [ ] Use data lineage tracking
- [ ] Implement anomaly detection in training data

## LLM04: Model Denial of Service
- [ ] Set input/output token limits
- [ ] Use rate limiting & resource quotas
- [ ] Monitor for resource exhaustion patterns

## LLM05: Supply Chain Vulnerabilities
- [ ] Verify model provenance & integrity (signatures)
- [ ] Scan plugins/extensions for vulnerabilities
- [ ] Use trusted model repositories

## LLM06: Sensitive Information Disclosure
- [ ] Apply data masking & redaction in prompts/outputs
- [ ] Implement PII detection filters
- [ ] Train users on safe prompting

## LLM07: Insecure Plugin Design
- [ ] Validate & authorize all plugin/tool calls
- [ ] Use least-privilege access tokens

## LLM08: Excessive Agency
- [ ] Define clear boundaries for autonomous actions
- [ ] Require human confirmation for high-impact actions

## LLM09: Overreliance
- [ ] Implement verification mechanisms for critical outputs
- [ ] Educate users on LLM limitations

## LLM10: Model Theft
- [ ] Protect model weights & inference endpoints
- [ ] Use watermarking & access controls

**Mapping to EU AI Act**:
- High-risk systems → Mandatory risk management covers most above.
- Use https://aiaudittool.net for automated OWASP + EU alignment checks.

**References**:
- Official: https://genai.owasp.org/llm-top-10/
- PDF: https://owasp.org/www-project-top-10-for-large-language-model-applications/assets/PDF/OWASP-Top-10-for-LLMs-v2025.pdf