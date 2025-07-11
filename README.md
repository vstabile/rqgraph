# RQGraph

**RQGraph** is a neural architecture grounded in an [informational theory of physics](https://www.texstr.org/a/naddr1qvzqqqr4gupzqwe6gtf5eu9pgqk334fke8f2ct43ccqe4y2nhetssnypvhge9ce9qqxnzde4xy6rydfcxqunsv35vk8jrc), where learning emerges from minimizing inconsistencies over loops in an informational graph.

Unlike traditional neural networks, RQGraph uses 2×2 Hermitian matrices as edge states between nodes representing informational degrees of freedom. Learning occurs by enforcing global consistency — minimizing Bures curvature over loops that connect inputs to class labels through internal structure.

---

## Biological Analogy

RQGraph mirrors how the brain may process information: inputs from the senses are encoded through fixed evolved biological filters (e.g., photoreceptors, cochlear hair cells), and enter the brain through dedicated boundary neurons. Rather than learning internal representations via backpropagation, the brain appears to rely on emergent coherence across recurrent loops and local consistency between pathways. RQGraph formalizes this idea: each input is injected into a specific position on the graph, and learning emerges from minimizing internal inconsistency across loops that involve inputs, internal processing, and expected outputs.

---

## Highlights

- **Informationally grounded**: Based on first principles of finite, relational, and consistent information.
- **Curvature-based learning**: Supervision is enforced via loop selection, not via gradients on labels.
- **Unconventional encoding**: Input features are directly encoded as edge relations to internal nodes.

---

## Architecture

- `Input Nodes`: One per feature (e.g., 4 for Iris).
- `Label Nodes`: One per class (3 in Iris).
- `Internal Nodes`: Shared nodes for relational inference.
- `Edges`: Learnable Hermitian 2×2 matrices; inputs encoded dynamically per sample.

---

## Dataset

This version uses the **Iris dataset**, where input features represent biologically encoded quantities (e.g., petal width). Features are normalized to the \([-1, 1]\) range to reflect limited sensory resolution and maintain geometric consistency.
