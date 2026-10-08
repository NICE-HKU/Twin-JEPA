<h1 align="center">TwinJEPA</h1>

<p align="center">
  <em>Action-Preferred Predictive Representations<br>for Goal-Conditioned Control</em>
</p>

<p align="center">
  <strong>Feiran You</strong> &nbsp;·&nbsp; <strong>Hongyang Du</strong><br>
  The University of Hong Kong
</p>

<p align="center">
  <a href="https://feiranyou.github.io/twinjepa/"><strong>Project page</strong></a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://arxiv.org/abs/2610.02922"><strong>Paper</strong></a>
</p>

<p align="center">
  TwinJEPA keeps the TD-JEPA backbone and adds offline-mined reward-gap<br>
  and preference supervision, with no extra cost at inference.
</p>

<p align="center">
  <img src="assets/figures/fig1_overview.png" alt="Figure 1. TwinJEPA overview." width="100%">
</p>

<p align="center">
  <strong>Figure 1.</strong>
  A temporal-prediction objective learns goal-conditioned structure.
  TwinJEPA mines action-diverse pairs and trains reward-gap and preference heads on one shared representation.
</p>

<h2 align="center">Environments</h2>

<p align="center">
  <img src="assets/figures/envs_all.png" alt="Environment views of AntMaze, Maze2D, Walker, Cheetah, and Quadruped." width="100%">
</p>

<table>
  <tr>
    <td align="center" width="20%"><img src="assets/figures/hero_tiles/antmaze.png" alt="AntMaze" width="100%"></td>
    <td align="center" width="20%"><img src="assets/figures/hero_tiles/maze2d.png" alt="Maze2D" width="100%"></td>
    <td align="center" width="20%"><img src="assets/figures/hero_tiles/walker.png" alt="Walker" width="100%"></td>
    <td align="center" width="20%"><img src="assets/figures/hero_tiles/cheetah.png" alt="Cheetah" width="100%"></td>
    <td align="center" width="20%"><img src="assets/figures/hero_tiles/quadruped.png" alt="Quadruped" width="100%"></td>
  </tr>
  <tr>
    <td align="center"><strong>AntMaze</strong><br><sub>OGBench</sub></td>
    <td align="center"><strong>Maze2D</strong><br><sub>D4RL</sub></td>
    <td align="center"><strong>Walker</strong><br><sub>DMC</sub></td>
    <td align="center"><strong>Cheetah</strong><br><sub>ExORL</sub></td>
    <td align="center"><strong>Quadruped</strong><br><sub>ExORL</sub></td>
  </tr>
</table>

<h2 align="center">Demos</h2>

<p align="center">
  Failure on the left, success on the right. Press play here, then open the project page for the matched figures and write-up.<br>
  <a href="https://feiranyou.github.io/twinjepa/#demos"><strong>Watch every demo on the project page</strong></a>
</p>

<h3 align="center">ExORL Quadruped · stand</h3>
<table>
  <tr>
    <td align="center" width="50%"><video src="https://github.com/user-attachments/assets/34423392-5052-4665-a13e-da7dcdf554f2" controls muted playsinline width="100%"></video></td>
    <td align="center" width="50%"><video src="https://github.com/user-attachments/assets/85837382-e934-4c5b-be83-2cd804553e2f" controls muted playsinline width="100%"></video></td>
  </tr>
  <tr>
    <td align="center"><strong>Low return</strong><br><sub>collapsed / unstable</sub></td>
    <td align="center"><strong>High return</strong><br><sub>upright torso</sub></td>
  </tr>
</table>

<h3 align="center">ExORL Cheetah · run</h3>
<table>
  <tr>
    <td align="center" width="50%"><video src="https://github.com/user-attachments/assets/e50b2b10-a91b-4e66-948c-4d5b36698b33" controls muted playsinline width="100%"></video></td>
    <td align="center" width="50%"><video src="https://github.com/user-attachments/assets/8ebf98b8-23c5-4cbd-a63a-dcd9d91273ec" controls muted playsinline width="100%"></video></td>
  </tr>
  <tr>
    <td align="center"><strong>Low return</strong><br><sub>little forward progress</sub></td>
    <td align="center"><strong>High return</strong><br><sub>forward locomotion</sub></td>
  </tr>
</table>

<h3 align="center">DMC Walker · walk</h3>
<table>
  <tr>
    <td align="center" width="50%"><video src="https://github.com/user-attachments/assets/76d3a460-d8b7-4857-90e9-6d88fb246fda" controls muted playsinline width="100%"></video></td>
    <td align="center" width="50%"><video src="https://github.com/user-attachments/assets/2529efd0-4921-4d7a-8fb9-7be6746c2637" controls muted playsinline width="100%"></video></td>
  </tr>
  <tr>
    <td align="center"><strong>Low return</strong><br><sub>from the offline buffer</sub></td>
    <td align="center"><strong>High return</strong><br><sub>upright forward gait</sub></td>
  </tr>
</table>

<h3 align="center">D4RL Maze2D · task 1</h3>
<table>
  <tr>
    <td align="center" width="50%"><video src="https://github.com/user-attachments/assets/dece16cb-3c8c-4238-bc8e-24129719d0a5" controls muted playsinline width="100%"></video></td>
    <td align="center" width="50%"><video src="https://github.com/user-attachments/assets/5db3e1c1-a8a6-4d6d-bbea-fd708da54a89" controls muted playsinline width="100%"></video></td>
  </tr>
  <tr>
    <td align="center"><strong>Miss</strong><br><sub>stays far from the goal</sub></td>
    <td align="center"><strong>Hit</strong><br><sub>enters the goal cell</sub></td>
  </tr>
</table>

<h3 align="center">OGBench AntMaze · task 1</h3>
<table>
  <tr>
    <td align="center" width="50%"><video src="https://github.com/user-attachments/assets/7db0c5d3-fe6c-4ee1-bf24-1d622f5060ed" controls muted playsinline width="100%"></video></td>
    <td align="center" width="50%"><video src="https://github.com/user-attachments/assets/04458f53-6044-4f4b-ae71-c9bbdff72764" controls muted playsinline width="100%"></video></td>
  </tr>
  <tr>
    <td align="center"><strong>Miss</strong><br><sub>never reaches the goal</sub></td>
    <td align="center"><strong>Hit</strong><br><sub>reaches the goal</sub></td>
  </tr>
</table>

<p align="center">
  <a href="https://feiranyou.github.io/twinjepa/"><strong>Project page</strong></a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://arxiv.org/abs/2610.02922"><strong>Paper</strong></a>
</p>
