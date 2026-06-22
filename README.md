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
- Paper: Understanding Certified Training with Interval Bound Propagation (https://arxiv.org/abs/2306.10426)
- How did CROWN-IBP develop further?
