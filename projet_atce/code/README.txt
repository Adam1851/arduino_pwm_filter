# Projet ATCE – Simulation PWM + Filtre RC

Ce projet est une simulation du comportement d’un signal PWM filtré par un passe-bas RC, dans le cadre du projet ATCE (Asservissement Temporel de Circuit Électronique).

# Contenu

- `arduino_pwm_filter.ino` : code Arduino simulant un signal PWM dont le rapport cyclique varie progressivement.
- `videos/` : dossier destiné à contenir les captures vidéo issues de SimulIDE montrant l’effet du filtrage RC.

# Objectif

L’objectif est d’observer le lissage d’un signal PWM à l’aide d’un filtre passe-bas composé d’une résistance de **10 kΩ** et d’un condensateur de **100 nF**, afin de produire une tension continue moyenne.

Ce montage est utilisé dans le projet pour piloter une varicap servant à ajuster la fréquence d’un oscillateur à quartz.

# Schéma de simulation

- Broche 9 de l’Arduino → Résistance 10 kΩ → Condensateur 100 nF vers la masse.
- Oscilloscope :
  - Canal 1 entre broche 9 et R (entrée du filtre)
  - Canal 2 après le condensateur (sortie filtrée)

# Simulation

La simulation a été réalisée dans **SimulIDE** avec une carte **Arduino UNO**.

# Auteurs

Projet réalisé en L3 SPI EA, UFRST, 2025.
