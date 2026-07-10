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
- References
Adversarial Training and Provable Defenses: Bridging the Gap (https://openreview.net/forum?id=SJxSDxrKDr)
- Certified Training: Small Boxes are All You Need (SABR)(https://arxiv.org/abs/2210.04871)
- Expressive Losses for Verified Robustness via Convex Combinations (https://proceedings.iclr.cc/paper_files/paper/2024/file/0b7dd2703eca7f58bae0bf455811b27e-Paper-Conference.pdf)
- TAPS: Connecting Certified and Adversarial Training. (https://arxiv.org/abs/2305.04574)
- Rethinking Lipschitz Neural Networks and Certified Robustness: A Boolean Function Perspective. (SortNet, https://arxiv.org/abs/2210.01787)
- Adversarial Training and Provable Robustness: A Tale of Two Objectives. (AdvIBP, https://arxiv.org/abs/2008.06081) 
- IBP Regularization for Verified Adversarial Robustness via Branch-and-Bound. (IBP-R, https://arxiv.org/abs/2210.01787)
- Learning Better Certified Models from Empirically-Robust Teachers (best robustness and acc atm what about the time doe,https://arxiv.org/pdf/2602.02626) 
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
### Application
- CertPHash: Towards Certified Perceptual Hashing via Robust Training : (https://www.usenix.org/conference/usenixsecurity25/presentation/yang-yuchen)
- Certified Robustness in Automated Driving Perception: 2025 : (they talk about verified robustness not certified kinda confusing, https://doi.org/10.1007/s42154-024-00347-3) 
- SoK: Certified Robustness for Deep Neural Networks (https://ieeexplore.ieee.org/document/10179303)
<img width="1433" height="595" alt="grafik" src="https://github.com/user-attachments/assets/b33976e5-2d55-4a6a-8fe9-8ade45ade37b" />
- CTBENCH: A Library and Benchmark for Certified Training (same infrastructure for all algorithms ,https://arxiv.org/pdf/2406.04848)


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

<img width="733" height="700" alt="grafik" src="https://github.com/user-attachments/assets/627f4dec-c8a1-48d5-9b46-a55b6e71820e" />
<img width="1284" height="466" alt="grafik" src="https://github.com/user-attachments/assets/c1ec5a39-cd6a-4a98-859c-e02843ffebe7" />

Bogen 1: Introduction — die Landkarte (deskriptiv)
Die Kernbewegung ist eine einzige: schrittweise Reduktion der Über-Regularisierung. Daran hängst du die Methoden als Stationen auf.

Startpunkt / Problem: Certified training braucht eine Approximation des intraktablen worst-case Loss. Der naheliegende Weg — sound over-approximation (IBP) — funktioniert für die Zertifizierung, aber die garantierte obere Schranke ist pessimistisch → Über-Regularisierung → schlechte Standard-Accuracy. Das ist die Spannung, die alles Folgende antreibt.
Erste Antwort — unsound approximations: Man opfert die Garantie im Training, um präziser zu approximieren. SABR (kleine Box um adversarialen Punkt), TAPS (IBP + latenter Angriff). Weniger Über-Regularisierung → bessere Accuracy und Certified.
Der Enabler (wichtig, gehört mit in den Bogen): Das ging nur, weil sich gleichzeitig die complete verifiers (branch-and-bound, α,β-CROWN) entwickelt haben — unsound-Netze sind mit billigem IBP nicht zertifizierbar. Trainings- und Verifikationsfortschritt bedingen sich.
Verallgemeinerung — expressive losses: Die einzelnen Heuristiken werden unter ein Prinzip gefasst (Interpolation adversarial↔verified über α\alpha
α). CC-IBP, MTL-IBP, Exp-IBP.
Jüngste Station — Distillation (CC-Dist): Selbst expressive losses schließen die Lücke zu empirischer Robustheit nicht. Also transferiert man die guten Repräsentationen eines empirisch-robusten Lehrers.
Abschluss des Bogens: Ein Satz, dass du diese Entwicklung in dieser Reihenfolge nachzeichnest.

Ton: behaupten, ordnen, orientieren. Keine Wertung, kein „aber". Die Intro erzählt die saubere Version.
Bogen 2: Discussion — die kritische Wendung (analytisch)
Hier nimmst du die scheinbar selbstverständliche Prämisse aus Bogen 1 und stellst sie in Frage. Die Kette:

Die implizite Annahme benennen: Der ganze sound→unsound-Fortschritt beruht auf einer Prämisse — präzisere worst-case-Loss-Approximation → bessere Performance. SABR und besonders TAPS begründen ihren Erfolg explizit damit (TAPS: „5-fold approximation error reduction" als zentrales Verkaufsargument).
Die Widerlegung: De Palma et al. (expressive losses) testen das direkt und finden: Das beste α\alpha
α entspricht nicht der besten Loss-Approximation (Abschnitt 6.3). Bei kleinen ϵ\epsilon
ϵ sind sogar über-approximierende Losses besser. Nicht Präzision zählt, sondern Expressivity — die Fähigkeit, überhaupt zwischen adversarial und verified zu interpolieren.
Die Konsequenz / Deutung: Das heißt, die Erfolgsgeschichte aus Bogen 1 stimmt im Ergebnis (die Methoden werden besser), aber die Begründung der Autoren (Präzision) ist vermutlich nicht der eigentliche Mechanismus. Der Fortschritt kam durch bessere Trade-off-Steuerung, nicht durch genaueres Treffen des worst case.
Optionaler zweiter Faden (verstärkt den kritischen Ton): Dazu passt, dass viel Erfolg in geteilter Infrastruktur steckt (Shi et al. Initialisierung, BatchNorm, ℓ1\ell_1
ℓ1​) statt in den namensgebenden Ideen — was die Frage aufwirft, wie viel jeder Einzelbeitrag wirklich beiträgt. Das ist dieselbe Skepsis gegenüber den behaupteten Erfolgsgründen.

Ton: hinterfragen, gegenüberstellen, urteilen. Hier ist das „aber" erlaubt, hier belegst du mit Tabellen.
