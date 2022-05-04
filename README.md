# LinkPrediction4SmallGraph
This repo is our work done in a project as coursework at university.

We apply GraphSAGE and GAT in a whole-batch forwarding manner, which is not advanced and optimized as implementation of PyTorch Geometric. Nonetheless, as expected, we obtained a significant improvement in AUC score.

If you want to re-use our code for your own dataset, please refer to notes in each section of the file `link_prediction.ipynb`. In summary, you need to rebuild the embedding for each node/datapoint of your dataset, then be able to directly apply our models.

Enjoying your project!
