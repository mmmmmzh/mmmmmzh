<h1 align="center">Hi, I'm May</h1>

<p align="center"><strong>World Models · Policy Learning · Autonomous Driving &amp; Embodied AI</strong></p>

<p align="center">
  <a href="https://github.com/mmmmmzh">GitHub</a> ·
  <a href="mailto:meizhehaoo@outlook.com">Email</a>
</p>

I study how learning-based agents **represent the world, improve their decisions, and adapt from limited experience**. My work connects world modeling and policy learning, with autonomous driving as a primary setting and robot manipulation as a complementary testbed.

## Research Directions

- **World models & dynamics** — Modeling how environments and vehicles respond to actions, and evaluating policies under changes in dynamics.
- **Planning & policy post-training** — Improving trajectory generators through supervised and reinforcement learning, with matched comparisons of driving progress and safety.
- **Embodied policy adaptation** — Studying how demonstration selection, data coverage, and execution feedback affect vision-language-action policies.

## Selected Research

| Project | My contribution | Results & evidence |
| :--- | :--- | :--- |
| **DrivoR post-training** | Implemented native trajectory-generator post-training, matched supervised/RL comparisons, and training-side experience replay. | Official evaluation over **12,146 scenes**: RL improved PDMS by **0.13481 percentage points** over matched supervised training. Single training seed; TTC remained below the original model. |
| **DynaDreamer reproduction** | Independently implemented dynamics-conditioned world modeling; built paired evaluation, checkpoint recovery, and environment diagnostics. | **120 frozen-policy episodes** across three training seeds: both methods reached the goal in **16/60** episodes. No arrival-rate advantage established; longer training was interrupted. |
| **π0.5 / LIBERO adaptation** | Built V100 adaptation and evaluation pipelines; studied learning-rate recipes, demonstration selection, data coverage, and observation frequency. | Three-seed recipe comparisons, **16,000 four-suite evaluations**, and **126 recovery-diagnostic rollouts**. Demonstration selection showed no verified advantage; recovery varied across training seeds. |

These are my implementation and evaluation studies built on the named prior methods. Research code is currently private. Detailed records are maintained with each project; paired behavior videos are available for DynaDreamer and VLA.

## Engineering

| Project | What I built | Availability |
| :--- | :--- | :--- |
| **[Fund Rebalance Agent](https://github.com/mmmmmzh/fund-rebalance-agent)** | An offline LangGraph workflow with human review, deterministic risk checks, audit logs, and a Streamlit interface. | **Public software demo**, using synthetic data; no trading-account connection. |

## Stack

`Python` · `PyTorch` · `JAX` · `CARLA` · `LIBERO` · `LangGraph` · `Streamlit`
