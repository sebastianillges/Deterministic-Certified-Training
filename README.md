# Deterministic-Certified-Training
ifftex : https://ifftex.fz-juelich.de/7142823159jhrjmscqbmbg#f14129

# Report Structure Outline
## Introduction: Why do we need Certified Training? (approx. 2 pages)
- Adversarial Examples
- (Empirical Robustness)
- (Adversarial Training)
- Problem: no guarantees
- Explain: why is normal robustness training not sufficient?
## Fundamentals: What is Certified Robustness? (clean distinction of terms)
- What is robustness?
- Local robustness
- Certified robustness
- (Verification)
- Certification
- Certified Training
## Certified Training
- How to realize certified training?
- We need:
  - (Methods for verification)
  - Bounds
  - ...
## IBP
- first really scalable method for certified training
- Explain:
  - Intervals
  - Bound propagation
  - Certified loss
  - advantages/disadvantages
## CROWN
- Why do intervals/bounds not suffice?
- Explain:
  - Convex relaxation
  - Linear bounds
  - Backward bounding
## CROWN-IBP (main paper, thus main chapter)
- Why combine both?
- Present results/performance
## Further developments/Outlook (small chapter)
- Paper: Fast Certified Robust Training with Short Warmup (https://arxiv.org/abs/2103.17268)
- Paper: Understanding Certified Training with Interval Bound Propagation (https://arxiv.org/abs/2306.10426) NOT SURE IF THATS RELEVANT FOR OUTLOOK THO
- How did CROWN-IBP develop further?

# SOTA Papers
## Important background papers
### Adversarial Examples
- Intriguing Properties of Neural Networks (https://arxiv.org/abs/1312.6199)
- Explaining and Harnessing Adversarial Examples (https://arxiv.org/abs/1412.6572)
### Adversarial Training
- Towards Deep Learning Models Resistant to Adversarial Attacks (https://arxiv.org/abs/1706.06083)
### Early Certified Defenses
- Provable Defenses via the Convex Outer Adversarial Polytope (https://arxiv.org/abs/1711.00851)
- Efficient Neural Network Robustness Certification with General Activation Functions (https://arxiv.org/abs/1811.00866)
### Interval Bound Propagation
- On the Effectiveness of Interval Bound Propagation for Training Verifiably Robust Models (https://arxiv.org/abs/1810.12715)
### CROWN-IBP
- Towards Stable and Efficient Training of Verifiably Robust Neural Networks (https://arxiv.org/abs/1906.06316)
## Core certified training papers
### IBP
- On the Effectiveness of Interval Bound Propagation for Training Verifiably Robust Models (https://arxiv.org/abs/1810.12715)
- Differentiable abstract interpretation for provably robust neural networks (https://proceedings.mlr.press/v80/mirman18b/mirman18b.pdf)
### CROWN
- Efficient Neural Network Robustness Certification with General Activation Functions (https://arxiv.org/abs/1811.00866)
### CROWN-IBP
- Towards Stable and Efficient Training of Verifiably Robust Neural Networks (https://arxiv.org/abs/1906.06316)
## Modern certified training papers
### Different Approach (also Bound propagation, just compared to IBP not to IBP-CROWN, mixed with adv training)
- Certified Training: Small Boxes are All You Need (SABR)(https://arxiv.org/abs/2210.04871)
- Expressive Losses for Verified Robustness via Convex Combinations (https://proceedings.iclr.cc/paper_files/paper/2024/file/0b7dd2703eca7f58bae0bf455811b27e-Paper-Conference.pdf)
- TAPS: Connecting Certified and Adversarial Training. (https://arxiv.org/abs/2305.04574)
- Rethinking Lipschitz Neural Networks and Certified Robustness: A Boolean Function Perspective. (SortNet, https://arxiv.org/abs/2210.01787)
- Adversarial Training and Provable Robustness: A Tale of Two Objectives. (AdvIBP, https://arxiv.org/abs/2008.06081) 
- IBP Regularization for Verified Adversarial Robustness via Branch-and-Bound. (IBP-R, https://arxiv.org/abs/2210.01787) 
### Fast Certified Training
- Fast Certified Robust Training with Short Warmup (https://arxiv.org/abs/2103.17268)

### Understanding IBP
- Understanding Certified Training with Interval Bound Propagation (https://arxiv.org/abs/2306.10426)
### Theoretical Analysis of Certified Training
- Certified Training: Small Boxes Are All You Need (https://arxiv.org/abs/2210.04871)
### Scaling Certified Training
- Automatic Perturbation Analysis for Scalable Certified Robustness and Beyond (https://arxiv.org/abs/2002.12920)
## Related infrastructure and framework papers
### Auto-LiRPA repository
- Auto-LiRPA (https://github.com/Verified-Intelligence/auto_LiRPA)
## Related verification papers
### Beta-CROWN
- Beta-CROWN: Efficient Bound Propagation with Per-neuron Split Constraints for Complete and Incomplete Neural Network Verification (https://arxiv.org/abs/2103.06624)
### Branch-and-Bound
- Branch and Bound for Piecewise Linear Neural Network Verification (https://arxiv.org/abs/1909.06588)
### Alpha-Beta-CROWN repository
- Alpha-Beta-CROWN (https://github.com/Verified-Intelligence/alpha-beta-CROWN)
### VNN-COMP
- International Verification of Neural Networks Competition (https://sites.google.com/view/vnn2025)



## Recommended reading order according to *AI*
### Stage 1: Motivation
- Intriguing Properties of Neural Networks
- Explaining and Harnessing Adversarial Examples
- Towards Deep Learning Models Resistant to Adversarial Attacks
### Stage 2: Certified robustness fundamentals
- Provable Defenses via the Convex Outer Adversarial Polytope
- Efficient Neural Network Robustness Certification with General Activation Functions
### Stage 3: Certified training
- On the Effectiveness of Interval Bound Propagation for Training Verifiably Robust Models
- Towards Stable and Efficient Training of Verifiably Robust Neural Networks
### Stage 4: Modern developments
- Understanding Certified Training with Interval Bound Propagation
- Certified Training: Small Boxes Are All You Need
- Fast Certified Robust Training with Short Warmup
### Stage 5: Optional verification deep dive
- Auto-LiRPA
- Beta-CROWN
- Branch and Bound for Piecewise Linear Neural Network Verification
