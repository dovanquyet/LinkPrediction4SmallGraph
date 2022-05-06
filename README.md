# LinkPrediction4SmallGraph
This repo is our work done in a project as coursework at university.

We apply GraphSAGE and GAT in a whole-batch forwarding manner, which is not advanced and optimized as implementation of PyTorch Geometric. Nonetheless, as expected, we obtained a significant improvement in AUC score, from .933 to .958.

|Models  | Score 
|--|--|
|DeepWalk (best)     | 0.9331 
|Node2Vec (p=1,q=2)   | 0.9321 
|MLP     | 0.9278 
|GraphSAGE   
|(1) src <- out, tar <- out    | 0.9546 
| ----- w/ no. hid. layer = 1  | 0.9529 
| ----- w/ hid. dim = 16   | 0.9535 
|(2) src <- in , tar <- out    | 0.9576
|(3) src <- out, tar <- in     | 0.9558 
|(4) src <- in , tar <- in     | 0.9551 
|(5) src <- all, tar <- all    | **0.9580**
|GAT     | 0.9372 

If you want to re-use our code for your own dataset, please refer to notes in each section of the file `link_prediction.ipynb`. In summary, you need to rebuild the embedding for each node/datapoint of your dataset, then be able to directly apply our models.

Enjoying your project!


#### Contribution
- `link_prediction.ipynb`: Quyet
- `visualization.ipynb`: Hoan
- `community_detection.ipynb`: Long
