---
title: PLEX: 'Making the Most of the Available Data for Robotic Manipulation Pretraining' layout: default
---

## Abstract
A rich representation is key to general robotic manipulation, but existing approaches to learning one require a lot of multimodal demonstrations.
In this work we propose PLEX, a transformer-based architecture that learns from a small amount of task-agnostic visuomotor trajectories accompanied by a much larger amount of task-conditioned object manipulation videos - a type of data that is available in quantity. The key insight behind PLEX is that visuomotor trajectories help induce a latent feature space and train a robot to execute task-agnostic manipulation routines, while diverse video-only demonstrations can efficiently teach the robot how to plan in this feature space for a wide variety of tasks. In contrast to most works on robotic manipulation pretraining, PLEX learns a generalizable sensorimotor multi-task policy, not just an observational representation. We also show that using relative positional encoding in PLEX's transformers greatly helps PLEX in low-data regimes when learning from human-collected demonstrations. Experiments showcase PLEX's generalization on the Meta-World-v2 benchmark and SOTA performance in challenging Robosuite environments.

<p align="center">
  <img src="https://user-images.githubusercontent.com/142258764/260860809-31243ea3-b7ad-47dd-baa8-66bdc0a1ec2f.png" alt="overview" width="70%">
</p>



## PLEX hyperparameter tuning experiments
<p align="center">
  <img src="https://user-images.githubusercontent.com/142258764/260900587-5363ea0d-07f9-453f-83af-c9d0ff57b95b.jpg" alt="overview" width="70%">
</p>


## MetaWorld playdata videos
<table align="center">
<tr>
  <td>bin-picking-v2</td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260901999-29e87c9e-f11f-44d6-8850-144fad81852a.mp4" type="video/mp4" controls></video></td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260902015-3d82c14d-2b36-4015-9504-cfb99276e09b.mp4" type="video/mp4" controls></video></td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260902024-e61f551c-c1f7-42ab-8ec0-42bddf56a63f.mp4" type="video/mp4" controls></video></td>
</tr>

<tr>
  <td>box-close-v2</td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260902901-6757d132-8d9a-419d-8dbc-325366ab972a.mp4" type="video/mp4" controls></video></td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260902009-812055b8-10e8-4249-859a-7276ab42bea8.mp4" type="video/mp4" controls></video></td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260902032-15574a1c-604c-4882-85e9-a6d7e37e8d51.mp4" type="video/mp4" controls></video></td>
</tr>

<tr>
  <td>door-lock-v2</td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260903783-a1a7c920-caaf-404d-b80c-0306baf26f7f.mp4" type="video/mp4" controls></video></td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260903795-7d839444-ea0c-4905-9bd4-1a49f5362f7e.mp4" type="video/mp4" controls></video></td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260903804-2fce55ec-40f5-4b17-a908-91303f7d6d20.mp4" type="video/mp4" controls></video></td>
</tr>

</table>

## Tasks on a real WidowX250 robot
<table>
<tr>
  <td>pick-and-place</td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260894005-6a1454e6-8c53-4326-ac9b-1cba49d5c033.mp4" type="video/mp4" controls></video></td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260894017-b980df07-4422-4fa8-95fb-be4d577a5c66.mp4" type="video/mp4" controls></video></td>
</tr>
  
<tr>
  <td>push-into-sink</td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260894202-8bb2a171-0eff-4e86-869e-b05c40d2d8ee.mp4" type="video/mp4" controls></video></td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260894218-c2959ac5-3582-48e3-a626-43be0ac4ecc7.mp4" type="video/mp4" controls></video></td>
</tr>

<tr>
  <td>lift-pan</td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260894261-cbc30fb3-1f4f-408b-ac33-f14557e16823.mp4" type="video/mp4" controls></video></td>
  <td><video width="168" height="168" src="https://user-images.githubusercontent.com/142258764/260894263-322e5b59-9f3e-42a3-a4ab-a8eaccbe1920.mp4" type="video/mp4" controls></video></td>
</tr>
</table>
