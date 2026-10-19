**The course’s central position is that AI models remain subject to the full model risk management (MRM) lifecycle, with additional controls for data dependence, opacity, bias, frequent retraining, and unpredictable outputs.** GenAI also requires governance of the surrounding system—prompts, retrieval pipelines, connected tools, and human interactions.

The extraction below focuses on those AI-specific requirements. References identify the module, section, and lesson in your document. “Requirements” means expectations expressed in the course; it does not imply that every item is a binding regulatory obligation.

### 1. AI/ML-specific requirements

| Area | Requirements extracted from the course | Source |
|---|---|---|
| **Model identification and inventory** | Assess AI applications against the institution’s model definition, including applications such as chatbots that do not produce conventional quantitative outputs. Record AI/ML classification, methodology complexity, data characteristics, output type, recalibration arrangements, dependencies, and appropriate monitoring metrics. | Module 5, §3.3, lesson 313 |
| **Model risk classification** | Assess materiality, complexity, and exposure. Consider opacity, ethical risks, bias, and recalibration when classifying AI models. Apply minimum model risk assessment standards even to models with low materiality. | Module 5, §§3.3 and 8.0, lessons 313, 338 |
| **Training and input data governance** | Evaluate data suitability, quality, provenance, permitted use, and treatment. Apply additional scrutiny to alternative data. Consider synthetic data and whether training data are accurate, sufficiently unbiased, structured, cleaned, and suitable for the task. | Module 5, §§2.1–2.5, lessons 301–305 |
| **Input data monitoring** | Monitor changes in data distributions, definitions, availability, and reporting practices. Outlier detection alone may be insufficient: changes disclosed by providers can affect model validity without appearing as obvious numerical anomalies. | Module 5, §2.2, lesson 302 |
| **Development and preprocessing controls** | Document data exclusions and their rationale; have humans examine automated exclusions that may remove useful information. Test and document transformations. Identify and prevent data leakage, justify model selection, and use appropriate training and cross-validation techniques. | Module 5, §4.0, lesson 316 |
| **Explainability and effective challenge** | Understand and challenge inputs, outputs, assumptions, and limitations even when model internals are opaque. Rigorously test outcomes and compare them with traditional models where possible. Balance predictive performance against interpretability and implementation burden. | Module 5, §§5.0 and 10.0, lessons 321, 346; Module 3, §§3.0–3.2, lessons 229–231 |
| **Performance evaluation** | Select metrics appropriate to the model type and business purpose; independent validation should assess their suitability. Use holdout samples, benchmarks, stress scenarios, and borderline cases. Adapt testing where conventional measures provide insufficient insight. | Module 5, §§3.3, 5.0 and 6.1, lessons 313, 321, 323 |
| **Bias and fairness assessment** | Examine bias arising from problem specification, features, data, development, and deployment. Assess outcomes across relevant populations. Justify fairness trade-offs: the course recognizes that all fairness definitions cannot generally be satisfied simultaneously. | Module 3, §§2.0–2.3.4, lessons 218–228; Module 4, §6.4, lesson 277 |
| **Monitoring and review frequency** | Use monitoring and review frequencies responsive to model risk, input changes, performance indicators, business volume, and external developments. AI/ML complexity and drift may warrant more frequent review than traditional models. | Module 5, §5.0, lesson 321 |
| **Retraining and change management** | Subject recalibration, retraining, rebuilding, and new uses to controlled change processes. Assess materiality and perform change-based validation when material. Prevent continuously learning models from moving into unvalidated states. | Module 5, §§3.4 and 5.0, lessons 314, 321 |
| **Accountability and control functions** | Retain first-line ownership, independent second-line challenge, and third-line assurance. Integrate monitoring into automated deployment pipelines. Involve additional functions—such as compliance, operational risk, and HR—where the application warrants them. | Module 5, §§3.4 and 5.0, lessons 314, 321 |
| **Validation expertise** | Provide validators with practical AI/ML expertise alongside statistical and business knowledge. Include familiarity with deployment platforms, cloud environments, MLOps, automated delivery pipelines, and model observability; supplement skills through training or specialists. | Module 5, §10.0, lesson 346 |

### 2. Additional requirements for GenAI

| Area | GenAI-specific expectation | Source |
|---|---|---|
| **Validation scope** | Address open-ended and unstructured outputs, hallucinations, bias, drift, data coverage, multimodal behavior, and limited explainability. Pay particular attention to open-source and third-party models. **Human review is explicitly described as essential to GenAI validation.** | Module 5, §6.1, lesson 323 |
| **Evaluation dimensions** | Assess content quality, factuality, hallucination propensity, robustness to unfamiliar inputs, adversarial robustness, jailbreak resistance, prompt sensitivity, fairness, and operational performance. | Module 2, §10.7, lesson 205 |
| **System-level governance** | Extend oversight beyond the underlying model to prompts, retrieval pipelines, connected data and tools, and human–AI interactions. Changes to these components can change performance. | Module 5, §9.1, lesson 340 |
| **Continuing assurance** | Combine initial and periodic validation with ongoing monitoring and checks at key changes. A one-time approval can become outdated as providers update models or capabilities change. | Module 5, §§9.0–9.2.1, lessons 339–342 |
| **Provider dependencies** | Understand provider update schedules, incident policies, allocation of responsibility, and relevant fine-tuning practices. Assess what is known about training data and alignment, and the institution’s control over the model. | Module 5, §§9.2.2 and 9.3, lessons 343, 345 |
| **Sensitive inputs and retention** | Trace how providers handle prompts and connected data, including storage, sharing, retention, and potential use for training. Apply controls to proprietary, confidential, and personal information. | Module 3, §9.2.2, lesson 251; Module 5, §9.3, lesson 345 |
| **Human oversight and use controls** | Define guardrails, human review triggers, usage limits, logging, ownership, and escalation arrangements appropriate to the application. Train staff to recognize hallucinations, data risks, and other problematic behavior. | Module 5, §§9.2.1 and 9.3, lessons 342, 345 |

### 3. Practices the course recommends, rather than universally mandates

The course presents the following as recommended or adaptable ways to implement these expectations:

- **Red-teaming and adversarial testing**, including prompt injection, chained prompts, unexpected queries, and edge cases.
- **Logs, audits, and feedback loops** to detect drift, misuse, and unexpected behavior after deployment.
- **Scenario plans and incident exercises** for hallucinations, misuse, and other unpredictable behavior.
- **Risk-based review gates**, with deeper review for high-impact or public-facing applications.
- **Watermarking where feasible**, to support content provenance.
- **Use of recognized frameworks**, such as NIST AI RMF and ISO/IEC 42001, to structure governance.

*Sources: Module 5, §4.1.1 and §§9.2.1–9.2.3, lessons 317, 342–344.*

### 4. Traditional MRM requirements that still apply

The document also carries forward the standard requirements for **documented purpose and approved use, independent validation before deployment, formal approval, use restrictions, ongoing monitoring, controlled changes, findings remediation, auditability, and retirement/decommissioning**. AI complexity or vendor opacity does not remove these responsibilities.

*Sources: Module 5, §§3.1–3.4, 4.2, 5.0 and 6.1, lessons 311–314, 320–323.*

One distinction matters when using this extraction: the course’s statements about data ownership, copyright, contractual indemnification, and regulatory obligations are **claims made by the supplied text**, not independently verified conclusions about current law.
