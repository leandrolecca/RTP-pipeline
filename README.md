[![Docker Pulls](https://img.shields.io/docker/pulls/scitran/afq-pipeline.svg)](https://hub.docker.com/r/scitran/afq-pipeline/)
[![Docker Stars](https://img.shields.io/docker/stars/scitran/afq-pipeline.svg)](https://hub.docker.com/r/scitran/afq-pipeline/)

## vistalab/RTP-pipeline
Reproducible Tract Profiles pipeline. 
Takes the preprocessed output from RTP-preproc and performs a series of operations:
1. Voxel level
    1. DTI
    2. CSD (single shell and multi-shell)
2. Tracking
3. Metrics
  1. DTI metrics for multishell cases are obtained in the shell closest to b=1000

It uses parts of these tools (depending on the options):
1. mrTrix 3 
2. mrDiffusion and AFQ
3. Ensemble Tractography (ET)
4. LiFE/SIFT2(TODO)
5. ANTs
6. SPM


TODO:
1. Add links and citations to external tools
2. Document all the options
3. It requires renaming of some of the parameters, right now some of the options are being used for both DTI and CSD and it can be confusing. 
4. Document how to download & use the Docker container locally without Flywheel. 
5. Document how to run it in Singularity; test/document it. 
