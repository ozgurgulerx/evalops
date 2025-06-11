# Core Components of Envelopes

This document is the main place for notes and explanations about the core components of envelopes. All relevant information and updates will be added here.

1. **Evaluation Dataset Management**: Managing test datasets for LLM evaluation is a foundational component. Unlike static ML tasks, generative AI requires *both static and dynamic* evaluation sets. A static test set (a fixed hold-out dataset) provides a consistent benchmark for comparing model versions.
. This is useful for regression testing – ensuring new model versions at least match or exceed prior performance on established examples. However, static sets alone can become stale or fail to represent evolving real-world 
. Thus, EvalOps also embraces dynamic and adaptive test sets. Dynamic evaluation means continually refreshing or expanding test cases based on model behavior and user data. For example, one can generate new adversarial or edge-case prompts dynamically based on prior model failures
. These adaptive benchmarks “keep evaluation a moving target” by challenging models in areas of weakness (e.g. automatically creating tougher questions or variations once a model masters easier ones)
. Additionally, production data plays a key role: logs of user queries and model responses can be recycled into “live” test sets to evaluate performance on actual usage scenarios
. In practice, a comprehensive EvalOps dataset strategy may include: 
- (a) a static core benchmark, 
- (b) a growing set of edge cases and failure-inducing queries, 
- (c) human-annotated examples for subjective or nuanced tasks, 
- (d) periodically sampled real user interactions

Combining these ensures broad coverage and keeps evaluations relevant as usage shifts over time.