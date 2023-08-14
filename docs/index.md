---
title: 'PLEX: Making the Most of the Available Data for Robotic Manipulation Pretraining' layout: default
---

<style>thead { display: none; }</style>

<p align="center">
  <img src="https://user-images.githubusercontent.com/142258764/260571799-a4b6a97d-d694-4c86-9abe-daf636e23c41.png" alt="overview" width="70%">
</p>

## Abstract
A rich representation is key to general robotic manipulation, but existing approaches to learning one require a lot of multimodal demonstrations.
In this work we propose PLEX, a transformer-based architecture that learns from a small amount of task-agnostic visuomotor trajectories accompanied by a much larger amount of task-conditioned object manipulation videos - a type of data that is available in quantity. The key insight behind PLEX is that visuomotor trajectories help induce a latent feature space and train a robot to execute task-agnostic manipulation routines, while diverse video-only demonstrations can efficiently teach the robot how to plan in this feature space for a wide variety of tasks. In contrast to most works on robotic manipulation pretraining, PLEX learns a generalizable sensorimotor multi-task policy, not just an observational representation. We also show that using relative positional encoding in PLEX's transformers greatly helps PLEX in low-data regimes when learning from human-collected demonstrations. Experiments showcase PLEX's generalization on the Meta-World-v2 benchmark and SOTA performance in challenging Robosuite environments.

## Videos
<table>
<tr>
  <td><video width="480" height="360" src="https://user-images.githubusercontent.com/142258764/260572315-ea1c03c9-8631-465e-a275-6bc470550738.mp4" type="video/mp4" controls></video></td>
</tr>
</table>

## Citation

If you reference or use PLEX in your research, please cite:

```bibtex
@misc{thomas2023plex,
      title={PLEX: Making the Most of the Available Data for Robotic Manipulation Pretraining}, 
      author={Garrett Thomas and Ching-An Cheng and Ricky Loynd and Felipe Vieira Frujeri Vibhav Vineet and Mihai Jalobeanu and Andrey Kolobov},
      year={2023},
      eprint={2303.08789},
      archivePrefix={arXiv},
      primaryClass={cs.RO}
}
```
