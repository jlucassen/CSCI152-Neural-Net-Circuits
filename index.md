## Inspecting Neural Network Reasoning Using Circuits

### Project Members
- James Lucassen
- Josh Cordova
- Sofiane Dissem
- Theo Bayard de Volo

### Outline
Neural networks are generally considered black boxes, which introduces a number of problems. If we do not understand the "reasoning" inside a neural network, we cannot necessarily trust it to be aligned, robust, or fair. [Previous research](https://distill.pub/2020/circuits/zoom-in/) has revealed that circuit analysiscan peer in to the black box of a neural net. Given that circuit analysis is a relatively new area of research, and the research up to this point has demonstrated the ability to uncover significant components of a neural network's reasoning, we believe that we can use these strategies on a smaller network to (near?) fully explain its behavior. One challenge we may run into is if there are no interpretable features in the output, as the circuit analysis expets interpretable features to be present but this is not guaranteed. As a target goal for this project, we expect to reasonably approximate the behavior of a simple vision model through circuit decomposition and recomposition.

### Ethics
If this project is successful, it could have substantial implications for data ethics. Transparency procedures are valuable for ensuring machine learning models act fairly, providing evidence in appeals against machine decisions, and a variety of other applications.
