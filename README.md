DL4J Examples 
=========================
*(based on version 0.0.3.3.\*)*

Repository of Deeplearning4J neural net examples:

- Convolutional Neural Nets
- Deep-belief Neural Nets
- Glove Example
- Restricted Boltzmann Machines
- Recurrent Neural Nets
- Recursive Neural Nets
- Word2Vec Examples (includes TSNE)

---
## Development
We are still developing and tuning these examples. If you notice issues, please log them, and if you want to contribute, submit a pull request. Input is welcome here.

Check the POM to confirm where these examples are running from. If it has SNAPSHOT in the dl4j and nd4j then *git clone* those repositories and build locally. Otherwise use Maven Repo. We are working to get this stabilized as quickly as possible.

## Documentation
For more information, check out [deeplearning4j.org](http://deeplearning4j.org/) and its [JavaDoc](http://deeplearning4j.org/doc/).

## Performance

| **Model Name**      | **Score** | **Status**   | **Training**  |
|---------------------|-----------|--------------|---------------|
| CNNIris             | F1 0.14   | Tune         | batch         |
| CNNMnist            | F1 0.02   | Tune         | batch         |
| CNNMnist2           | F1 0.02   | Tune         | batch         |
| DBNCreateData       | F1 0.33   | Tune         | batch         |          	
| DBNFullMnist        | F1 0.18   | Tune         | full          |
| DBNIris             | F1 0.15   | Tune         | full          |
| DBNLWF              | F1 0.0    | Tune         | batch         |
| DBNMnistRecontruct  | F1 0.017  | Tune         | batch         |
| DBNSmallMnist       | F1 0.02   | Tune         | full          |
| GloveRawSentence    | Sim 0     | Tune         | batch         |
| MLPBackpropIris     | F1 0.16   | Tune         | batch         |
| RBMCreateData	      | NA        | Validate     | full          |
| RBMIris             | NA        | Validate     | full          |
| RecurrentLSTMMnist  | NA        | Validate     | batch         |
| RecursiveAutoEncoder| NA        | Validate     | batch         |
| RNTNTweets          | F1 0.48   | Tune         | batch         |
| RNTNTweets2         | F1 0.48   | Tune         | batch         |
| TSNEBarnesHut       | NA        | Validate     | NA            |
| TSNEStandard        | NA        | Validate     | NA            |
| Word2VecRawText     | Sim 0     | Tune         | batch         |
    

F1 scores vary with each run. We're starting to add **rng** to help stabilize results. Some examples still require an rng fix. 
