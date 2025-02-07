## Functional Requirements

The company wants to invest in owning its infrastructure rather than relying on cloud-managed services.

**Key reasons for this decision:**

- **Privacy concerns**: The organization wants full control over user data, avoiding potential exposure to third-party providers.
- **Cost control**: There is concern that the cost of managed GenAI services could significantly increase over time, making self-hosting a more predictable and sustainable solution.

### Infrastructure Investment

- The company plans to invest in an **AI PC** with a budget of **$10,000–$15,000** to support in-house GenAI workloads.
- The system should be capable of running an **open-source LLM** efficiently while keeping **operational costs minimal**.
- The company has **300 active students**, all located within **Koto-ku, Tokyo**.

## Assumptions

- The selected **open-source LLM** will be powerful enough to run effectively on the **$10K–$15K hardware** investment.
- A **single server connected to the internet** will be sufficient to serve **300 students** without major performance or bandwidth limitations.
- Internet bandwidth will be adequate for handling inference requests, model updates, and other required operations.
- The company will have the necessary technical expertise to manage and maintain on-premises AI infrastructure.

## Data Strategy

- Due to concerns about **copyrighted material**, the company must ensure compliance by **purchasing and legally sourcing** all educational materials.
- These materials will be **stored securely** in an internal database and will be accessible by the AI system for training and inference.
- The organization will establish **clear policies** to prevent unauthorized use of copyrighted content.

## Conceptual Architecture

![Architecture](./genai-architecting.png)

## Considerations

- The company is considering using **IBM Granite**, as it is a **truly open-source model** with **traceable training data**. This ensures:
  - **Transparency**: The organization knows what data the model was trained on, reducing risks of legal or ethical concerns.
  - **Avoidance of copyright issues**: Since the training data is publicly documented, there is less risk of accidentally using copyrighted material.
  - **Full control over the model**: The model can be fine-tuned or modified without vendor lock-in.
  - IBM Granite Model: [Hugging Face Repository](https://huggingface.co/ibm-granite)

### Additional Considerations

- **Model Performance & Scalability**: The chosen model must be optimized to run on the AI PC while maintaining response time and efficiency.
- **Power & Cooling**: Running an AI workload in-house requires **adequate power supply and cooling** solutions to prevent hardware degradation.
- **Security Measures**:
  - Data encryption and **access control policies** should be implemented to **protect user information**.
  - Secure **API endpoints** should be established for student interactions with the AI system.
- **Long-Term Maintenance**: The organization must allocate resources for ongoing model updates, hardware maintenance, and system monitoring.
