# Biformer
 TensorFlow and Keras Implementation of the paper - BiFormer: Vision Transformer with Bi-Level Routing Attention
 
 Paper : https://arxiv.org/pdf/2303.08810.pdf
 
 Abstract :
 
 As the core building block of vision transformers, attention is a powerful tool to capture long-range dependency.
However, such power comes at a cost: it incurs a huge
computation burden and heavy memory footprint as pairwise token interaction across all spatial locations is computed. A series of works attempt to alleviate this problem
by introducing handcrafted and content-agnostic sparsity
into attention, such as restricting the attention operation to
be inside local windows, axial stripes, or dilated windows.
In contrast to these approaches, we propose a novel dynamic sparse attention via bi-level routing to enable a more
flexible allocation of computations with content awareness.
Specifically, for a query, irrelevant key-value pairs are first
filtered out at a coarse region level, and then fine-grained
token-to-token attention is applied in the union of remaining candidate regions (i.e., routed regions). We provide
a simple yet effective implementation of the proposed bilevel routing attention, which utilizes the sparsity to save
both computation and memory while involving only GPUfriendly dense matrix multiplications. Built with the proposed bi-level routing attention, a new general vision transformer, named BiFormer, is then presented. As BiFormer
attends to a small subset of relevant tokens in a query adaptive manner without distraction from other irrelevant ones,
it enjoys both good performance and high computational
efficiency, especially in dense prediction tasks. Empirical
results across several computer vision tasks such as image
classification, object detection, and semantic segmentation
verify the effectiveness of our design


