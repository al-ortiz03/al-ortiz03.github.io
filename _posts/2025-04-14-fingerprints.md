## Matching Fingerprints with a GUI

> Part one of this assignment was to create a GUI enabling a user to enrol a fingerprint in the database, then compare other fingerprints.

### Performance
ROC curves allow the evaluation of classification model performance by graphing true match rate against false match rate. 

![](/images/Example1.png "Fingerprint Comparison 1")

The ROC curve below is for the implemented fingerprint system. Evidently, the curve is questionable but modifying graph generation to achieve a better curve was unsuccessful. It can be concluded that the model has a relatively consistent true match rate over most thresholds, except for very low ones where a lot of false positives occur. 




### Challenges
A challenge was setting the threshold, as even correct matches often had relatively low scores of around 0.6 - 0.7.  
It was decided to leave it up to the user, although this is obviously not feasible in real applications - the user could just set it to zero.

### Examples
Below are some examples of matching fingerprints, captured at different angles, and a mismatched fingerprint.

![](/images/Example1.png "Fingerprint Comparison 1")
![](/images/Example2.png "Fingerprint Comparison 2 - Same database image, new comparison image")

Fingerprint mismatches can be detected by large distances between minutiae pairs and crossing lines.


![](/images/Mismatch.png "Mismatched fingerprints")



