## Inspecting Neural Network Reasoning Using Circuits

### Project Members
- James Lucassen
- Josh Cordova
- Sofiane Dissem
- Theo Bayard de Volo

### Outline
Neural networks are generally considered black boxes, which introduces a number of problems. If we do not understand the "reasoning" inside a neural network, it makes it much harder to verify whether it is aligned, robust, or fair. [Previous research](https://distill.pub/2020/circuits/) has revealed that circuit analysis can peer into the black box of a neural net. Given that circuit analysis is a relatively new area of research, and the research up to this point has demonstrated the ability to uncover significant components of a neural network's reasoning, we believe that we can use these strategies on a smaller network to (near?) fully explain its behavior. One challenge we may run into is if there are no interpretable features in the output, as the existing circuits literature suggests interpretable features will be present but this is not guaranteed. As a target goal for this project, we expect to reasonably approximate the behavior of a simple vision model through circuit decomposition and recomposition. If this project is successful, it could have substantial implications for data ethics. Transparency procedures are valuable for ensuring machine learning models act fairly before deployment, providing evidence in appeals against unfair machine decisions, and a variety of other applications.

### Literature Review
1. [Feature Visualization](https://distill.pub/2017/feature-visualization/): This paper describes one of the key methods of circuit analysis - feature visualization by image optimization. Visualization by optimization allows for a more precise understanding of a feature than simply selecting high-activation images because it removes features that may be irrelevant but correlated - especially when multiple diverse outputs can be compared to identify the commonality. The authors highlight that a variety of regularization techniques are required before this method produces coherent results, otherwise the output tends to be full of high-frequency noise and resemble an adversarial example more than a feature visualization.
2. [Curve Circuits](https://distill.pub/2020/circuits/curve-circuits/): In this paper researchers use neural circuits to isolate, identify, and group the steps InceptionV1 uses to detect curves. They then verify their claims by creating an artificial artificial network from the isolated circuits that identifies curves in a very similar way to the original model. Finally, the reasearches discuss the role these isolated cicuits play in indentifying more complex visual artifacts downstream in InceptionV1.
3. 
4. [Visualizing Weights](https://distill.pub/2020/circuits/visualizing-weights/): This paper describes multiple techniques for specifically visualizing weights.
The main technique is decomposing features into their corresponding weight vectors, however it assumes that there is little non-linear interaction between layers. Still, the "expanded weights" method, which replaces non-linear operations with the closest linear operation, is able to identify meaningful interactions between layers.

