# New Gain

This project offers improvements based on Generative Adversarial Imputation Networks (GAIN)
Reference: J. Yoon, J. Jordon, M. van der Schaar, "GAIN: Missing Data Imputation using Generative Adversarial Nets," ICML, 2018.
[Paper](http://medianetlab.ee.ucla.edu/papers/ICML_GAIN.pdf)
[Appendix](http://medianetlab.ee.ucla.edu/papers/ICML_GAIN_Supp.pdf)

All code is derived from the work written by Yoon et al. https://bitbucket.org/mvdschaar/mlforhealthlabpub/src/master/alg/gain/ and https://github.com/jsyoon0823/GAIN/blob/master/gain.py Contact: jsyoon0823@g.ucla.edu


## Example usage:



```
    python3 create_missing.py --dataset bc -o missing.csv --oref ref.csv --istarget 1 --normalize01 1
    python3 gain.py -i missing.csv -o imputed.csv --target target
    python3 gain_ana.py -i missing.csv --ref ref.csv --imputed imputed.csv -o result.json --target target
```
or just:
```
    bash run.sh
```

