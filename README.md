# Causal-GAIL
Code for Causal GAIL

## Major Difference between GAIL and Causal-GAIL

tl;dr:
- In \cite{ruan2022learning}, to block all the $\pi$-backdoor paths in the proposed causal template for human driving behaviors, we need to utilize 2-step information, i.e., $\\{S_{t}, A_{t-1}, S_{t-1} \\}$.
  - Causal GAIL: $\pi(a_{t} | s_{t}, a_{t-1}, s_{t-1})$
  - Original GAIL: $\pi(a_{t} | s_{t})$
- In \cite{ruan2023causal}, we need to utilize the minimal $\pi$-backdoor criterion.



## References

If you found this library useful in your research, please consider citing our papers:
```bib
@inproceedings{ruan2022learning,
  title={Learning human driving behaviors with sequential causal imitation learning},
  author={Ruan, Kangrui and Di, Xuan},
  booktitle={Proceedings of the AAAI Conference on Artificial Intelligence},
  volume={36},
  number={4},
  pages={4583--4592},
  year={2022}
}


@inproceedings{
    ruan2023causal,
    title={Causal Imitation Learning via Inverse Reinforcement Learning},
    author={Kangrui Ruan and Junzhe Zhang and Xuan Di and Elias Bareinboim},
    booktitle={The Eleventh International Conference on Learning Representations },
    year={2023},
    url={https://openreview.net/forum?id=B-z41MBL_tH}
}
```