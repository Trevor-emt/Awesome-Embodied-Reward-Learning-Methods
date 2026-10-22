# Awesome Embodied Reward Learning Methods

A curated reading list accompanying **A Survey of Embodied Rewards for Robotic Manipulation**. This list follows the four reward families and subsection structure of the survey version dated **October 22, 2026**.

The collection covers **119 distinct papers** on reward construction, including the methodological precursors discussed in the survey. Papers are organized by their primary reward supervision: desired outcomes, task progress, demonstrated behavior, and comparative judgments.

## Contents

- [Goal-oriented Rewards](#goal-oriented-rewards)
  - [Goal-reaching Outcome as Reward](#goal-reaching-outcome-as-reward)
  - [Spatial Distance as Reward](#spatial-distance-as-reward)
  - [Latent Distance as Reward](#latent-distance-as-reward)
- [Progress-oriented Rewards](#progress-oriented-rewards)
  - [Absolute Progress Estimation](#absolute-progress-estimation)
  - [Relative Progress Estimation](#relative-progress-estimation)
  - [Stage- and Procedure-Aware Progress Estimation](#stage--and-procedure-aware-progress-estimation)
- [Distribution-oriented Rewards](#distribution-oriented-rewards)
  - [Distribution Matching As Explicit Discrimination](#distribution-matching-as-explicit-discrimination)
  - [Predictive Expert Modeling as Implicit Discrimination](#predictive-expert-modeling-as-implicit-discrimination)
  - [Reference-Conditioned Sequence Matching as Approximate Discrimination](#reference-conditioned-sequence-matching-as-approximate-discrimination)
- [Preference-oriented Rewards](#preference-oriented-rewards)
  - [Preferences from Human Feedback](#preferences-from-human-feedback)
  - [Synthetic Preference Construction](#synthetic-preference-construction)
  - [Preferences from Foundation Model Feedback](#preferences-from-foundation-model-feedback)

## Reading Notes

- Classification follows the survey. Within each subsection, papers are sorted by year (oldest first), then alphabetically by their full titles within the same year, ignoring case, spaces, and punctuation.
- Papers discussed in multiple subsections are cross-listed. Repeated entries refer to the same paper.
- **Paper** links lead to a publication page, an arXiv record, or an author-hosted paper. **Code** and **Website** links are included only when an author-associated implementation or project page was identified.
- An omitted Code or Website link means that no confirmed resource was found, not necessarily that none exists. Code marked as coming soon is not listed.
- General-purpose perception models, datasets, pure theoretical references, and non-embodied action-progress background papers are not listed as reward methods.
- Years follow the survey bibliography; publication years may differ from arXiv submission dates. Some OpenReview paper links may require browser verification.


## Goal-oriented Rewards

### Goal-reaching Outcome as Reward

| Year | Paper | Links |
| --- | --- | --- |
| 2019 | **EDRIAD**: A Practical Approach to Insertion with Variable Socket Position Using Deep Reinforcement Learning | [Paper](https://arxiv.org/abs/1810.01531) &middot; [Website](https://sites.google.com/view/dpgfd-insertion/home) |
| 2019 | **VICE-RAQ**: End-To-End Robotic Reinforcement Learning without Reward Engineering | [Paper](https://arxiv.org/abs/1904.07854) &middot; [Code](https://github.com/avisingh599/reward-learning-rl) &middot; [Website](https://sites.google.com/view/reward-learning-rl/) |
| 2022 | **LOReL**: Learning Language-Conditioned Robot Behavior from Offline Data and Crowd-Sourced Annotation | [Paper](https://proceedings.mlr.press/v164/nair22a.html) &middot; [Code](https://github.com/suraj-nair-1/lorel) &middot; [Website](https://sites.google.com/view/robotlorel) |
| 2023 | **SuccessVQA**: Vision-Language Models as Success Detectors | [Paper](https://proceedings.mlr.press/v232/du23b.html) |
| 2024 | **RoboFuME**: Robot Fine-Tuning Made Easy: Pre-Training Rewards and Policies for Autonomous Real-World Reinforcement Learning | [Paper](https://arxiv.org/abs/2310.15145) &middot; [Website](https://robofume.github.io/) |
| 2025 | **GenReward**: Goal-Driven Reward by Video Diffusion Models for Reinforcement Learning | [Paper](https://arxiv.org/abs/2512.00961) &middot; [Code](https://github.com/qiwang067/GenReward) &middot; [Website](https://qiwang067.github.io/genreward) |
| 2026 | **VLA-MBPO**: Towards Practical World Model-based Reinforcement Learning for Vision-Language-Action Models | [Paper](https://arxiv.org/abs/2603.20607) &middot; [Code](https://github.com/LAMDA-RL/VLA-MBPO) &middot; [Website](https://rhx11111.github.io/VLA-MBPO/) |

### Spatial Distance as Reward

| Year | Paper | Links |
| --- | --- | --- |
| 2018 | **Visual Foresight**: Model-Based Deep Reinforcement Learning for Vision-Based Robotic Control | [Paper](https://arxiv.org/abs/1812.00568) &middot; [Code](https://github.com/SudeepDasari/visual_foresight) &middot; [Website](https://sites.google.com/view/visualforesight/home) |
| 2020 | Object-Centric Forward Modeling for Model Predictive Control | [Paper](https://proceedings.mlr.press/v100/ye20a.html) &middot; [Website](https://judyye.github.io/ocmpc/) |
| 2021 | **S3K**: Self-Supervised Semantic Keypoints for Robotic Manipulation via Multi-View Consistency | [Paper](https://proceedings.mlr.press/v155/vecerik21a.html) &middot; [Website](https://sites.google.com/view/2020-s3k/home) |
| 2024 | **Code as Reward**: Empowering Reinforcement Learning with VLMs | [Paper](https://proceedings.mlr.press/v235/venuto24a.html) &middot; [Code](https://github.com/dvVenuto/vlm-car) |
| 2025 | **KAGI**: Affordance-Guided Reinforcement Learning via Visual Prompting | [Paper](https://arxiv.org/abs/2407.10341) &middot; [Website](https://sites.google.com/view/affordance-guided-rl) |
| 2025 | **IKER**: A Real-to-Sim-to-Real Approach to Robotic Manipulation with VLM-Generated Iterative Keypoint Rewards | [Paper](https://arxiv.org/abs/2502.08643) &middot; [Website](https://xinchenyin.github.io/iker.github.io/) |
| 2025 | Crossing the Human-Robot Embodiment Gap with Sim-to-Real RL Using One Human Demonstration | [Paper](https://proceedings.mlr.press/v305/lum25a.html) &middot; [Code](https://github.com/tylerlum/human2sim2robot) &middot; [Website](https://human2sim2robot.github.io/) |
| 2025 | **APS-Net**: Learning Efficient Robotic Garment Manipulation with Standardization | [Paper](https://proceedings.mlr.press/v267/zhou25q.html) &middot; [Website](https://hellohaia.github.io/APS/) |
| 2025 | **Points2Reward**: Robotic Manipulation Rewards from Just One Video | [Paper](https://points2reward.github.io/static/Points2Reward.pdf) &middot; [Website](https://points2reward.github.io/) |
| 2025 | Scaffolding Dexterous Manipulation with Vision-Language Models | [Paper](https://arxiv.org/abs/2506.19212) &middot; [Code](https://github.com/vdebakker/vlm-scaffolding) &middot; [Website](https://sites.google.com/view/dexterous-vlm-scaffolding) |
| 2026 | **ReLAM**: Learning Anticipation Model for Rewarding Visual Robotic Manipulation | [Paper](https://proceedings.mlr.press/v306/tang26o.html) |
| 2026 | **VLS**: Steering Pretrained Robot Policies via Vision-Language Models | [Paper](https://arxiv.org/abs/2602.03973) &middot; [Code](https://github.com/Vision-Language-Steering/code) &middot; [Website](https://vision-language-steering.github.io/webpage/) |

### Latent Distance as Reward

| Year | Paper | Links |
| --- | --- | --- |
| 2018 | **RIG**: Visual Reinforcement Learning with Imagined Goals | [Paper](https://arxiv.org/abs/1807.04742) &middot; [Code](https://github.com/rail-berkeley/rlkit) &middot; [Website](https://sites.google.com/site/visualrlwithimaginedgoals/) |
| 2020 | **CC-RIG**: Contextual Imagined Goals for Self-Supervised Robotic Learning | [Paper](https://proceedings.mlr.press/v100/nair20a.html) &middot; [Code](https://github.com/anair13/rlkit/tree/ccrig/examples/ccrig) &middot; [Website](https://ccrig.github.io/) |
| 2021 | Learning Predictive Representations for Deformable Objects Using Contrastive Estimation | [Paper](https://proceedings.mlr.press/v155/yan21a.html) &middot; [Code](https://github.com/wilson1yan/contrastive-forward-model) &middot; [Website](https://sites.google.com/view/contrastive-predictive-model) |
| 2021 | **ROLL**: Visual Self-Supervised Reinforcement Learning with Object Reasoning | [Paper](https://proceedings.mlr.press/v155/wang21e.html) &middot; [Code](https://github.com/yufeiwang63/ROLL) &middot; [Website](https://sites.google.com/andrew.cmu.edu/roll/home) |
| 2022 | **ZeST**: Can Foundation Models Perform Zero-Shot Task Specification for Robot Manipulation? | [Paper](https://arxiv.org/abs/2204.11134) &middot; [Website](https://sites.google.com/view/zestproject) |
| 2022 | **XIRL**: Cross-Embodiment Inverse Reinforcement Learning | [Paper](https://proceedings.mlr.press/v164/zakka22a.html) &middot; [Website](https://x-irl.github.io/) |
| 2022 | **Grounded-NL-R**: Zero-Shot Reward Specification via Grounded Natural Language | [Paper](https://proceedings.mlr.press/v162/mahmoudieh22a.html) |
| 2023 | Graph Inverse Reinforcement Learning from Diverse Videos | [Paper](https://proceedings.mlr.press/v205/kumar23a.html) &middot; [Code](https://github.com/SateeshKumar21/graph-inverse-rl) &middot; [Website](https://graphirl.github.io/) |
| 2023 | **LIV**: Language-Image Representations and Rewards for Robotic Control | [Paper](https://arxiv.org/abs/2306.00958) &middot; [Code](https://github.com/penn-pal-lab/LIV) &middot; [Website](https://penn-pal-lab.github.io/LIV) |
| 2023 | **VIP**: Towards Universal Visual Reward and Representation via Value-Implicit Pre-Training | [Paper](https://arxiv.org/abs/2210.00030) &middot; [Code](https://github.com/facebookresearch/vip) |
| 2023 | **CLIP-ZS**: Vision-Language Models as a Source of Rewards | [Paper](https://arxiv.org/abs/2312.09187) |
| 2024 | **Adapt2Reward**: Adapting Video-Language Models to Generalizable Robotic Rewards via Failure Prompts | [Paper](https://arxiv.org/abs/2407.14872) |
| 2024 | **DecisionNCE**: Embodied Multimodal Representations via Implicit Preference Learning | [Paper](https://proceedings.mlr.press/v235/li24cr.html) &middot; [Code](https://github.com/2toinf/DecisionNCE) &middot; [Website](https://2toinf.github.io/DecisionNCE/) |
| 2024 | **VLM-RM**: Vision-Language Models are Zero-Shot Reward Models for Reinforcement Learning | [Paper](https://arxiv.org/abs/2310.12921) &middot; [Code](https://github.com/AlignmentResearch/vlmrm) |
| 2025 | **DINO-WM**: World Models on Pre-Trained Visual Features Enable Zero-Shot Planning | [Paper](https://proceedings.mlr.press/v267/zhou25t.html) &middot; [Code](https://github.com/gaoyuezhou/dino_wm) &middot; [Website](https://dino-wm.github.io/) |
| 2025 | **GoalLadder**: Incremental Goal Discovery with Vision-Language Models | [Paper](https://arxiv.org/abs/2506.16396) |
| 2025 | **PLDM**: Learning from Reward-Free Offline Data: A Case for Planning with Latent Dynamics Models | [Paper](https://arxiv.org/abs/2502.14819) &middot; [Code](https://github.com/vladisai/PLDM) &middot; [Website](https://latent-planning.github.io/) |
| 2025 | **GCR**: On-Robot Reinforcement Learning with Goal-Contrastive Rewards | [Paper](https://arxiv.org/abs/2410.19989) &middot; [Website](https://gcr-robot.github.io/) |
| 2025 | **VICtoR**: Learning Hierarchical Vision-Instruction Correlation Rewards for Long-Horizon Manipulation | [Paper](https://arxiv.org/abs/2405.16545) &middot; [Code](https://github.com/cmlab-victor/victor-code) |
| 2025 | **VIRL**: Self-Supervised Visual Graph Inverse Reinforcement Learning | [Paper](https://proceedings.mlr.press/v270/huang25d.html) &middot; [Website](https://leihhhuang.github.io/VIRL/) |
| 2025 | **WorldPlanner**: Monte Carlo Tree Search and MPC with Action-Conditioned Visual World Models | [Paper](https://arxiv.org/abs/2511.03077) |
| 2026 | **LeWorldModel**: Stable End-to-End Joint-Embedding Predictive Architecture from Pixels | [Paper](https://arxiv.org/abs/2603.19312) &middot; [Code](https://github.com/lucas-maes/le-wm) &middot; [Website](https://le-wm.github.io/) |
| 2026 | **MVR**: Multi-view Video Reward Shaping for Reinforcement Learning | [Paper](https://arxiv.org/abs/2603.01694) &middot; [Code](https://github.com/mvr-rl/mvr) &middot; [Website](https://mvr-rl.github.io/) |
| 2026 | **Reward-Zero**: Language Embedding Driven Implicit Reward Mechanisms for Reinforcement Learning | [Paper](https://arxiv.org/abs/2603.09331) |
| 2026 | **RMTL**: Reinforced Micro-task Learning for Long-Horizon Manipulation with VLM Rewards | [Paper](https://arxiv.org/abs/2606.26175) |
| 2026 | **Temporal-Distance JEPA**: Plan-Aware Representation Learning for Latent World Model Predictive Control | [Paper](https://arxiv.org/abs/2607.25337) &middot; [Code](https://github.com/HKBU-KnowComp/Temporal-Distance-JEPA) |
| 2026 | Temporal Straightening for Latent Planning | [Paper](https://proceedings.mlr.press/v306/wang26n.html) &middot; [Code](https://github.com/agentic-learning-ai-lab/temporal-straightening/) |

<!-- ### Goal Specification and Acquisition

| Year | Paper | Links |
| --- | --- | --- |
| 2018 | **Visual Foresight**: Model-Based Deep Reinforcement Learning for Vision-Based Robotic Control | [Paper](https://arxiv.org/abs/1812.00568) &middot; [Code](https://github.com/SudeepDasari/visual_foresight) &middot; [Website](https://sites.google.com/view/visualforesight/home) |
| 2018 | **RIG**: Visual Reinforcement Learning with Imagined Goals | [Paper](https://arxiv.org/abs/1807.04742) &middot; [Code](https://github.com/rail-berkeley/rlkit) &middot; [Website](https://sites.google.com/site/visualrlwithimaginedgoals/) |
| 2019 | **VICE-RAQ**: End-To-End Robotic Reinforcement Learning without Reward Engineering | [Paper](https://arxiv.org/abs/1904.07854) &middot; [Code](https://github.com/avisingh599/reward-learning-rl) &middot; [Website](https://sites.google.com/view/reward-learning-rl/) |
| 2019 | **Hierarchical Visual Foresight**: Hierarchical Foresight: Self-Supervised Learning of Long-Horizon Tasks via Visual Subgoal Generation | [Paper](https://arxiv.org/abs/1909.05829) |
| 2020 | **CC-RIG**: Contextual Imagined Goals for Self-Supervised Robotic Learning | [Paper](https://proceedings.mlr.press/v100/nair20a.html) &middot; [Code](https://github.com/anair13/rlkit/tree/ccrig/examples/ccrig) &middot; [Website](https://ccrig.github.io/) |
| 2023 | **LfVoid**: Can Pre-Trained Text-to-Image Models Generate Visual Goals for Reinforcement Learning? | [Paper](https://arxiv.org/abs/2307.07837) &middot; [Code](https://github.com/gaojl19/LfVoid) &middot; [Website](https://lfvoid-rl.github.io/) |
| 2023 | **LIV**: Language-Image Representations and Rewards for Robotic Control | [Paper](https://arxiv.org/abs/2306.00958) &middot; [Code](https://github.com/penn-pal-lab/LIV) &middot; [Website](https://penn-pal-lab.github.io/LIV) |
| 2024 | **Adapt2Reward**: Adapting Video-Language Models to Generalizable Robotic Rewards via Failure Prompts | [Paper](https://arxiv.org/abs/2407.14872) |
| 2024 | **DecisionNCE**: Embodied Multimodal Representations via Implicit Preference Learning | [Paper](https://proceedings.mlr.press/v235/li24cr.html) &middot; [Code](https://github.com/2toinf/DecisionNCE) &middot; [Website](https://2toinf.github.io/DecisionNCE/) |
| 2024 | **VLM-RM**: Vision-Language Models are Zero-Shot Reward Models for Reinforcement Learning | [Paper](https://arxiv.org/abs/2310.12921) &middot; [Code](https://github.com/AlignmentResearch/vlmrm) |
| 2025 | **KAGI**: Affordance-Guided Reinforcement Learning via Visual Prompting | [Paper](https://arxiv.org/abs/2407.10341) &middot; [Website](https://sites.google.com/view/affordance-guided-rl) |
| 2025 | **GenReward**: Goal-Driven Reward by Video Diffusion Models for Reinforcement Learning | [Paper](https://arxiv.org/abs/2512.00961) &middot; [Code](https://github.com/qiwang067/GenReward) &middot; [Website](https://qiwang067.github.io/genreward) |
| 2025 | **GoalLadder**: Incremental Goal Discovery with Vision-Language Models | [Paper](https://arxiv.org/abs/2506.16396) |
| 2025 | **Points2Reward**: Robotic Manipulation Rewards from Just One Video | [Paper](https://points2reward.github.io/static/Points2Reward.pdf) &middot; [Website](https://points2reward.github.io/) |
| 2025 | **RL with Anticipation**: Reinforcement Learning with Anticipation: A Hierarchical Approach for Long-Horizon Tasks | [Paper](https://arxiv.org/abs/2509.05545) |
| 2025 | **VICtoR**: Learning Hierarchical Vision-Instruction Correlation Rewards for Long-Horizon Manipulation | [Paper](https://arxiv.org/abs/2405.16545) &middot; [Code](https://github.com/cmlab-victor/victor-code) |
| 2026 | **Anticipation-VLA**: Solving Long-Horizon Embodied Tasks via Anticipation-based Subgoal Generation | [Paper](https://arxiv.org/abs/2605.01772) |
| 2026 | **ReLAM**: Learning Anticipation Model for Rewarding Visual Robotic Manipulation | [Paper](https://proceedings.mlr.press/v306/tang26o.html) |
| 2026 | **Reward-Zero**: Language Embedding Driven Implicit Reward Mechanisms for Reinforcement Learning | [Paper](https://arxiv.org/abs/2603.09331) |
| 2026 | **RMTL**: Reinforced Micro-task Learning for Long-Horizon Manipulation with VLM Rewards | [Paper](https://arxiv.org/abs/2606.26175) | -->

## Progress-oriented Rewards

### Absolute Progress Estimation

| Year | Paper | Links |
| --- | --- | --- |
| 2021 | **Goal-Prox**: Generalizable Imitation Learning from Observation via Inferring Goal Proximity | [Paper](https://papers.nips.cc/paper/2021/hash/868b7df964b1af24c8c0a9e43a330c6a-Abstract.html) &middot; [Code](https://github.com/clvrai/goal_prox_il) |
| 2025 | **PROGRESSOR**: A Perceptually Guided Reward Estimator with Self-Supervised Online Refinement | [Paper](https://arxiv.org/abs/2411.17764) &middot; [Code](https://github.com/ripl/progressor) &middot; [Website](https://ripl.github.io/progressor/) |
| 2025 | **ReWiND**: Language-Guided Rewards Teach Robot Policies without New Demonstrations | [Paper](https://arxiv.org/abs/2505.10911) &middot; [Code](https://github.com/rewind-reward/ReWiND) |
| 2025 | **GVL**: Vision Language Models are In-Context Value Learners | [Paper](https://arxiv.org/abs/2411.04549) |
| 2026 | **DenseReward**: Dense Reward Learning via Failure Synthesis for Robotic Manipulation | [Paper](https://arxiv.org/abs/2607.13033) &middot; [Code](https://github.com/dense-reward/dense-reward) &middot; [Website](https://dense-reward.github.io/) |
| 2026 | **Large Reward Models**: Generalizable Online Robot Reward Generation with Vision-Language Models | [Paper](https://arxiv.org/abs/2603.16065) &middot; [Code](https://github.com/physical-superintelligence-lab/Large-Reward-Models/) &middot; [Website](https://yanru-wu.github.io/Large-Reward-Models/) |
| 2026 | **ProgAgent**: A Continual RL Agent with Progress-Aware Rewards | [Paper](https://arxiv.org/abs/2603.07784) |
| 2026 | **ProgressLM**: Towards Progress Reasoning in Vision-Language Models | [Paper](https://arxiv.org/abs/2601.15224) &middot; [Code](https://github.com/ProgressLM/ProgressLM) |
| 2026 | **ProgressVLA**: Progress-Guided Diffusion Policy for Vision-Language Robotic Manipulation | [Paper](https://arxiv.org/abs/2603.27670) |
| 2026 | **Robometer**: Scaling General-Purpose Robotic Reward Models via Trajectory Comparisons | [Paper](https://arxiv.org/abs/2603.02115) &middot; [Code](https://github.com/robometer/robometer) |
| 2026 | **RoboReward**: General-Purpose Vision-Language Reward Models for Robotics | [Paper](https://arxiv.org/abs/2601.00675) &middot; [Website](https://crfm.stanford.edu/helm/robo-reward-bench/) |
| 2026 | **UR-VC**: Unsupervised Robotic Value Correction for Time-Derived Progress Proxies | [Paper](https://arxiv.org/abs/2607.12892) &middot; [Website](https://liruizhao.com/projects/UR-VC/) |

### Relative Progress Estimation

| Year | Paper | Links |
| --- | --- | --- |
| 2020 | **Reward Sketching**: Scaling Data-Driven Robotics with Reward Sketching and Batch Reinforcement Learning | [Paper](https://arxiv.org/abs/1909.12200) &middot; [Website](https://sites.google.com/view/data-driven-robotics/) |
| 2024 | **Rank2Reward**: Learning Shaped Reward Functions from Passive Video | [Paper](https://arxiv.org/abs/2404.14735) &middot; [Code](https://github.com/dxyang/rank2reward) |
| 2026 | **VLAC**: A Generalist Pair-wise Progress Critic Model for Vision-Language-Action Robots | [Paper](https://proceedings.mlr.press/v306/zhang26if.html) &middot; [Code](https://github.com/InternRobotics/VLAC) |
| 2026 | **ARM**: Advantage Reward Modeling for Long-Horizon Manipulation | [Paper](https://arxiv.org/abs/2604.03037) &middot; [Code](https://github.com/aiming1998/ARM) &middot; [Website](https://aiming1998.github.io/ARM/) |
| 2026 | **Robo-Dopamine**: General Process Reward Modeling for Robotic Reinforcement Learning | [Paper](https://openaccess.thecvf.com/content/CVPR2026/html/Tan_General_Process_Reward_Modeling_for_Robotic_Reinforcement_Learning_CVPR_2026_paper.html) &middot; [Code](https://github.com/FlagOpen/Robo-Dopamine) &middot; [Website](https://robo-dopamine.github.io/) |
| 2026 | **Large Reward Models**: Generalizable Online Robot Reward Generation with Vision-Language Models | [Paper](https://arxiv.org/abs/2603.16065) &middot; [Code](https://github.com/physical-superintelligence-lab/Large-Reward-Models/) &middot; [Website](https://yanru-wu.github.io/Large-Reward-Models/) |
| 2026 | **RARM**: Confidence-Gated Progress Reward Modeling for RL in Manipulation | [Paper](https://arxiv.org/abs/2606.22027) &middot; [Website](https://rarm-robotics.github.io/) |
| 2026 | **TimeRewarder**: Learning Dense Reward from Passive Videos via Frame-wise Temporal Distance | [Paper](https://proceedings.mlr.press/v306/liu26et.html) &middot; [Website](https://timerewarder.github.io/) |

### Stage- and Procedure-Aware Progress Estimation

| Year | Paper | Links |
| --- | --- | --- |
| 2017 | **Unsup-PR**: Unsupervised Perceptual Rewards for Imitation Learning | [Paper](https://arxiv.org/abs/1612.06699) &middot; [Website](https://sermanet.github.io/rewards/) |
| 2022 | Visual Rewards From Observation for Sequential Tasks: Autonomous Pile Loading | [Paper](https://www.frontiersin.org/journals/robotics-and-ai/articles/10.3389/frobt.2022.838059/full) |
| 2024 | **DrS**: Learning Reusable Dense Rewards for Multi-Stage Tasks | [Paper](https://arxiv.org/abs/2404.16779) &middot; [Code](https://github.com/tongzhoumu/DrS) &middot; [Website](https://sites.google.com/view/iclr24drs) |
| 2025 | **DEMO<sup>3</sup>**: Multi-Stage Manipulation with Demonstration-Augmented Reward, Policy, and World Model Learning | [Paper](https://proceedings.mlr.press/v267/escoriza25a.html) &middot; [Code](https://github.com/adrialopezescoriza/demo3) &middot; [Website](https://sites.google.com/view/icml2025demo3) |
| 2025 | **PRM4RL**: Progress Reward Model for Reinforcement Learning via Large Language Models | [Paper](https://arxiv.org/abs/2610.22056) &middot; [Code](https://github.com/deng-ai-lab/PRM4RL) |
| 2025 | **ROVER**: Recursive Reasoning Over Videos with Vision-Language Models for Embodied Tasks | [Paper](https://arxiv.org/abs/2508.01943) &middot; [Code](https://github.com/Philip-MIT/rover-vlm) &middot; [Website](https://rover-vlm.github.io/) |
| 2025 | **REDS**: Subtask-Aware Visual Reward Learning from Segmented Demonstrations | [Paper](https://arxiv.org/abs/2502.20630) &middot; [Code](https://github.com/csmile-1006/REDS_agent) |
| 2025 | **VICtoR**: Learning Hierarchical Vision-Instruction Correlation Rewards for Long-Horizon Manipulation | [Paper](https://arxiv.org/abs/2405.16545) &middot; [Code](https://github.com/cmlab-victor/victor-code) |
| 2026 | **VLLR**: Generalizable Dense Reward for Long-Horizon Robotic Tasks | [Paper](https://arxiv.org/abs/2604.00055) |
| 2026 | **ProcVLM**: Learning Procedure-Grounded Progress Rewards for Robotic Manipulation | [Paper](https://arxiv.org/abs/2605.08774) &middot; [Code](https://github.com/RUCKBReasoning/ProcVLM) &middot; [Website](https://procvlm.github.io/) |
| 2026 | **R<sup>2</sup>VLM**: Recurrent Reasoning with Vision-Language Models for Estimating Long-Horizon Embodied Task Progress | [Paper](https://arxiv.org/abs/2603.17312) &middot; [Code](https://github.com/GLAD-RUC/R2VLM) |
| 2026 | **SARM2**: Multi-Task Stage Aware Reward Modeling for Self Improving Robotic Manipulation | [Paper](https://arxiv.org/abs/2606.10305) &middot; [Code](https://github.com/xdofai/opensarm) &middot; [Website](https://qianzhong-chen.github.io/sarm2.github.io/) |
| 2026 | **SARM**: Stage-Aware Reward Modeling for Long Horizon Robot Manipulation | [Paper](https://arxiv.org/abs/2509.25358) &middot; [Code](https://github.com/xdofai/opensarm) &middot; [Website](https://qianzhong-chen.github.io/sarm.github.io/) |
| 2026 | Stage-Transition Dense Reward Modeling for Reinforcement Learning | [Paper](https://arxiv.org/abs/2606.31377) |

## Distribution-oriented Rewards

### Distribution Matching As Explicit Discrimination

| Year | Paper | Links |
| --- | --- | --- |
| 2016 | **GAIL**: Generative Adversarial Imitation Learning | [Paper](https://arxiv.org/abs/1606.03476) &middot; [Code](https://github.com/openai/imitation) |
| 2019 | **GAIfO**: Generative Adversarial Imitation from Observation | [Paper](https://arxiv.org/abs/1807.06158) |
| 2021 | **V-MAIL**: Visual Adversarial Imitation Learning Using Variational Models | [Paper](https://arxiv.org/abs/2107.08829) &middot; [Code](https://github.com/rmrafailov/VMAIL) &middot; [Website](https://sites.google.com/view/variational-mail) |
| 2023 | **PatchAIL**: Visual Imitation Learning with Patch Rewards | [Paper](https://arxiv.org/abs/2302.00965) &middot; [Code](https://github.com/sail-sg/PatchAIL) |
| 2024 | **LAIfO**: Adversarial Imitation Learning from Visual Observations Using Latent Information | [Paper](https://arxiv.org/abs/2309.17371) |
| 2025 | **C-LAIfO**: Visually Robust Adversarial Imitation Learning from Videos with Contrastive Learning | [Paper](https://arxiv.org/abs/2407.12792) |
| 2026 | **MPAIL<sup>2</sup>**: Online World Modeling Enables Real-World Inverse Reinforcement Learning from Observation | [Paper](https://arxiv.org/abs/2602.24121) &middot; [Code](https://github.com/UWRobotLearning/mpail2) &middot; [Website](https://uwrobotlearning.github.io/mpail2/) |
| 2026 | **CoPT-AIL**: Provably Efficient Policy-Reward Co-Pretraining for Adversarial Imitation Learning | [Paper](https://proceedings.mlr.press/v306/xu26j.html) &middot; [Code](https://github.com/LAMDA-RL/CoPT-AIL) |

### Predictive Expert Modeling as Implicit Discrimination

| Year | Paper | Links |
| --- | --- | --- |
| 2023 | **VIPER**: Video Prediction Models as Rewards for Reinforcement Learning | [Paper](https://arxiv.org/abs/2305.14343) &middot; [Code](https://github.com/escontra/viper_rl) |
| 2024 | **Diffusion Reward**: Learning Rewards via Conditional Video Diffusion | [Paper](https://arxiv.org/abs/2312.14134) &middot; [Code](https://github.com/TEA-Lab/diffusion_reward) &middot; [Website](https://diffusion-reward.github.io/) |
| 2025 | **ActionSink**: Toward Precise Robot Manipulation with Dynamic Integration of Action Flow | [Paper](https://arxiv.org/abs/2508.03218) |
| 2026 | **Dream2Reward**: Transition-Alignment Reward Models from Positive Demonstrations for Robotic Manipulation | [Paper](https://arxiv.org/abs/2608.18787) |
| 2026 | **Motion Prediction Reward**: Human Preference Modeling Using Visual Motion Prediction Improves Robot Skill Learning from Egocentric Human Video | [Paper](https://arxiv.org/abs/2602.11393) |
| 2026 | **XIPER**: Reinforcement Learning from Cross-Domain Videos with Video Prediction Model | [Paper](https://arxiv.org/abs/2606.03201) &middot; [Code](https://github.com/yangzhao-666/xiper) &middot; [Website](https://sites.google.com/view/xiper) |

### Reference-Conditioned Sequence Matching as Approximate Discrimination

| Year | Paper | Links |
| --- | --- | --- |
| 2021 | **P-SIL**: Imitation Learning from Pixel Observations for Continuous Control | [Paper](https://openreview.net/forum?id=Xe5MFhFvYGX) |
| 2021 | **DVD**: Learning Generalizable Robotic Reward Functions from "In-The-Wild" Human Videos | [Paper](https://arxiv.org/abs/2103.16817) &middot; [Code](https://github.com/anniesch/dvd) |
| 2023 | **RoboCLIP**: One Demonstration is Enough to Learn Robot Policies | [Paper](https://arxiv.org/abs/2310.07899) &middot; [Code](https://github.com/sumedh7/RoboCLIP/) |
| 2023 | **ROT**: Watch and Match: Supercharging Imitation with Regularized Optimal Transport | [Paper](https://proceedings.mlr.press/v205/haldar23a.html) &middot; [Code](https://github.com/siddhanthaldar/ROT) &middot; [Website](https://rot-robot.github.io/) |
| 2024 | **TemporalOT**: Robot Policy Learning with Temporal Optimal Transport Reward | [Paper](https://arxiv.org/abs/2410.21795) &middot; [Code](https://github.com/fuyw/TemporalOT) &middot; [Website](https://sites.google.com/site/hczhang1/projects/temporalot) |
| 2025 | **ORCA**: Imitation Learning from a Single Temporally Misaligned Video | [Paper](https://proceedings.mlr.press/v267/huey25a.html) &middot; [Code](https://github.com/portal-cornell/orca/) &middot; [Website](https://portal-cornell.github.io/orca/) |

## Preference-oriented Rewards

### Preferences from Human Feedback

| Year | Paper | Links |
| --- | --- | --- |
| 2017 | Deep Reinforcement Learning from Human Preferences | [Paper](https://arxiv.org/abs/1706.03741) |
| 2018 | Reward Learning from Human Preferences and Demonstrations in Atari | [Paper](https://arxiv.org/abs/1811.06521) |
| 2022 | **IBT**: Improving Multimodal Interactive Agents with Reinforcement Learning from Human Feedback | [Paper](https://arxiv.org/abs/2211.11602) |
| 2023 | Learning a Universal Human Prior for Dexterous Manipulation from Human Preference | [Paper](https://arxiv.org/abs/2304.04602) |
| 2024 | **RAPL**: Maximizing Alignment with Minimal Feedback: Efficiently Learning Rewards for Visuomotor Robot Policy Alignment | [Paper](https://arxiv.org/abs/2412.04835) &middot; [Website](https://sites.google.com/berkeley.edu/rapl/home) |
| 2025 | **FDPP**: Fine-Tune Diffusion Policy with Human Preference | [Paper](https://arxiv.org/abs/2501.08259) |
| 2025 | **HALO**: Human Preference Aligned Offline Reward Learning for Robot Navigation | [Paper](https://proceedings.mlr.press/v305/seneviratne25a.html) |
| 2026 | **FPL**: Freeform Preference Learning for Robotic Manipulation | [Paper](https://arxiv.org/abs/2606.32027) &middot; [Code](https://github.com/freeform-pl/fpl) &middot; [Website](https://freeform-pl.github.io/fpl.website/) |

### Synthetic Preference Construction

| Year | Paper | Links |
| --- | --- | --- |
| 2020 | **D-REX**: Better-than-Demonstrator Imitation Learning via Automatically-Ranked Demonstrations | [Paper](https://proceedings.mlr.press/v100/brown20a.html) &middot; [Code](https://github.com/dsbrown1331/CoRL2019-DREX) &middot; [Website](https://dsbrown1331.github.io/CoRL2019-DREX/) |
| 2022 | **SURF**: Semi-Supervised Reward Learning with Data Augmentation for Feedback-Efficient Preference-Based Reinforcement Learning | [Paper](https://arxiv.org/abs/2203.10050) &middot; [Code](https://github.com/alinlab/SURF) |
| 2023 | **LERP**: Learning Noise-Induced Reward Functions for Surpassing Demonstrations in Imitation Learning | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/25962) |
| 2023 | **STRAPPER**: Preference-Based Reinforcement Learning via Self-Training Augmentation and Peer Regularization | [Paper](https://arxiv.org/abs/2307.09692) |
| 2024 | **PEARL**: Zero-Shot Cross-Task Preference Alignment and Robust Reward Learning for Robotic Manipulation | [Paper](https://arxiv.org/abs/2306.03615) &middot; [Website](https://sites.google.com/view/pearl-preference) |
| 2025 | **APEC**: Improving Reward Model Generalization from Adversarial Process Enhanced Preferences | [Paper](https://proceedings.mlr.press/v267/zhang25ci.html) &middot; [Code](https://github.com/Zzl35/APEC) |
| 2025 | **VLP**: Vision-Language Preference Learning for Embodied Manipulation | [Paper](https://aclanthology.org/2025.emnlp-main.1444/) &middot; [Website](https://vlpref.github.io/) |
| 2026 | **VOTP**: Video-Based Optimal Transport for Feedback-Efficient Offline Preference-Based Reinforcement Learning | [Paper](https://proceedings.mlr.press/v306/luu26a.html) &middot; [Code](https://github.com/tunglm2203/votp) &middot; [Website](https://votp2026.github.io/) |

### Preferences from Foundation Model Feedback

| Year | Paper | Links |
| --- | --- | --- |
| 2024 | **RL-VLM-F**: Reinforcement Learning from Vision Language Foundation Model Feedback | [Paper](https://arxiv.org/abs/2402.03681) &middot; [Code](https://github.com/yufeiwang63/RL-VLM-F) &middot; [Website](https://rlvlmf2024.github.io/) |
| 2025 | **PRIMT**: Preference-Based Reinforcement Learning with Multimodal Feedback and Trajectory Synthesis from Foundation Models | [Paper](https://arxiv.org/abs/2509.15607) &middot; [Website](https://primt25.github.io/) |
| 2025 | **Offline RL-VLM-F**: Real-World Offline Reinforcement Learning from Vision Language Model Feedback | [Paper](https://arxiv.org/abs/2411.05273) &middot; [Website](https://offline-rlvlmf.github.io/) |
| 2025 | **TREND**: Tri-Teaching for Robust Preference-Based Reinforcement Learning with Demonstrations | [Paper](https://arxiv.org/abs/2505.06079) &middot; [Website](https://shuaiyihuang.github.io/publications/TREND/) |
| 2025 | **VARP**: Reinforcement Learning from Vision-Language Model Feedback with Agent Regularized Preferences | [Paper](https://arxiv.org/abs/2503.13817) |
