# LunarLander DQN

This is my personal DQN project for LunarLander (via `gymnasium`) — TensorFlow-based, notebook-driven, and meant for tinkering.

## What's here
- `main.ipynb`: training + eval + video recording
- `q_network.h5`, `target_q_network.h5`: saved networks
- `videos/`: evaluation clips (mp4)

## Quick setup
Create a venv and install the essentials:

```powershell
python -m venv .venv; .\.venv\Scripts\Activate.ps1
pip install -U pip
pip install gymnasium[box2d] tensorflow numpy
```

Run `main.ipynb` to train or eval; the notebook uses `RecordVideo` and drops MP4s into `videos/`.

## Learning-progress clips
Here are a few representative eval clips from the training run — early → mid → later. Playable in the README (if your browser supports MP4):

### Episode 0 — very early
<video width="420" controls>
  <source src="videos/dqn_lander-episode-0.mp4" type="video/mp4">
  Your browser does not support embedded videos.
</video>

### Episode 10 — mid training
<video width="420" controls>
  <source src="videos/dqn_lander-episode-10.mp4" type="video/mp4">
  Your browser does not support embedded videos.
</video>

### Episode 29 — later / best-ish
<video width="420" controls>
  <source src="videos/dqn_lander-episode-29.mp4" type="video/mp4">
  Your browser does not support embedded videos.
</video>

