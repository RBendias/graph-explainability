# Master Thesis: Understanding Explainability Methods for Graph Neural Networks

As Graph Neural Networks (GNNs) are increasingly used in critical applications, numerous methods for interpreting these models have been presented in recent years. Furthermore, traditional machine learning explanation approaches can also be extended for use on GNNs. To facilitate the deployment of generic explanation techniques, we design an interface that enables the application of Captum explanation methods to PyG GNNs without requiring additional code changes. Both generic and graph-specific explanation strategies must be thoroughly validated in order to be used reliably. To this point, however, there are no standardized procedures for that purpose available. Therefore, we create benchmarks with datasets that have been generated according to mathematical rules. Using these rules, we derive ground truth explanations for edges, entire nodes, and node features. We investigate the explanation methods GNNExplainer, PGExplainer, Guided Backpropagation, GradientShap, Lime, Integrated Gradients (IG), and Saliency on their performance for GNNs. These methods are applied to the graph models SumGNN, GCN, PNA, and GraphSAGE. First, we find that the GNN-specific algorithms GNNExplainer and PGExplainer cannot provide explanations corresponding to ground truth values. In contrast, IG and GradientShap detect important and unimportant edges, nodes, and node features, especially for the PNA model, and outperform all other explanation methods.

## Citation
```
@mastersthesis{Bendias22,
  title={{Understanding Explainability Methods for Graph Neural Networks}},
  author={Ramona Bendias},
  school={Technische Universit{\"a}t Berlin},
  year={2022},
}
