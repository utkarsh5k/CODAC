# Conservative Distributional Offline Reinforcement Learning

This is the PARK related fork for [Conservative Distributional Offline Reinforcement Learning](https://arxiv.org/abs/2107.06106).
Currently the repository is in active development and there are things to be fixed: 

Tasks: 

- [x] Port CODAC to run with PARK
- [x] Use risk penalty and risk probability in PARK environments 
- [ ] Verify and implement which dataset to be loaded, right now the train_offline script loads the epoch1 run, which should be changed. 

## Installations

The park-codac.yml file contains the conda environment. You can create this environment using the provided yml file. 

## Experiments

Right now the repository is tested on the load balance environment. 

For online training: 

```python train_online.py --env load_balance --algo codac```

Then you can run offline training: 

```python train_offline.py --env load_balance --algo codac```

## Citations
If you find this repository useful for your research, please cite:
```
@article{ma2021conservative,
      title={Conservative Offline Distributional Reinforcement Learning}, 
      author={Yecheng Jason Ma and Dinesh Jayaraman and Osbert Bastani},
      year={2021},
      url={https://arxiv.org/abs/2107.06106}
}
```

## Contact
If you have any questions regarding the code or paper, feel free to contact me at jasonyma@seas.upenn.edu or open an issue on this repository.
## Acknowledgement
This repository contains code adapted from the 
following repositories: [pytorch-soft-actor-critic](https://github.com/pranz24/pytorch-soft-actor-critic),
 [CQL](https://github.com/aviralkumar2907/CQL), [dsac](https://github.com/xtma/dsac), [focops](https://github.com/ymzhang01/mujoco-circle) and [replication-mbpo](https://github.com/jxu43/replication-mbpo). We thank the
 authors and contributors for open-sourcing their code.  
