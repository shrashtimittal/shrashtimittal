<div align="center">

<img src="assets/header/hero.svg" width="100%" alt="Shrashti Mittal, Aerospace Engineer. Spacecraft systems, mission analysis and robotics. MSc student at Sapienza University of Rome. A spacecraft flies a Hohmann transfer orbit.">

**[Projects](#featured-projects)** &nbsp;·&nbsp; **[Robotics](#robotics)** &nbsp;·&nbsp; **[Research](#research)** &nbsp;·&nbsp; **[Skills](#skills)** &nbsp;·&nbsp; **[GitHub](https://github.com/shrashtimittal?tab=repositories)** &nbsp;·&nbsp; **[Contact](#contact)**

</div>

I am an aerospace engineer, currently an MSc student in **Space and Astronautical Engineering at Sapienza University of Rome**. I work across spacecraft systems, mission analysis, robotics and computational research: I frame a problem, model and simulate it, build the software or hardware, and record honestly what the results do and do not show.

<a name="engineering-focus"></a>
<img src="assets/sections/engineering-focus.svg" width="100%" alt="01 Engineering focus">

<table>
<tr>
<td width="50%" valign="top"><img src="assets/icons/space.svg" width="36" alt=""><br><b>Space systems and mission engineering</b><br>Spacecraft design, mission analysis, orbital mechanics, navigation, satellite and CubeSat systems.</td>
<td width="50%" valign="top"><img src="assets/icons/robotics.svg" width="36" alt=""><br><b>Robotics and embedded systems</b><br>UAVs, flight controllers, microcontrollers, sensor integration and autonomous systems.</td>
</tr>
<tr>
<td valign="top"><img src="assets/icons/compute.svg" width="36" alt=""><br><b>Computational engineering and AI</b><br>Scientific computing, simulation, modelling and machine learning for engineering problems.</td>
<td valign="top"><img src="assets/icons/research.svg" width="36" alt=""><br><b>Scientific research</b><br>Astrophysics and dark matter, quantum and theoretical physics, orbital and navigation concepts.</td>
</tr>
</table>

<a name="featured-projects"></a>
<img src="assets/sections/featured-projects.svg" width="100%" alt="02 Featured projects">

Each description was checked against the repository's code. Simulations here are not flight-tested systems.

### QRNG Spacecraft Navigation
<a href="https://github.com/shrashtimittal/qrng-spacecraft-navigation"><img src="assets/diagrams/qrng-pipeline.svg" width="100%" alt="Simulation pipeline: bit source, Gaussian noise model, measurements, Kalman filter and RMSE, with a circular truth orbit."></a>

**Question:** does the source of randomness (classical pseudo-random or quantum-sourced bits) change how simulated measurement noise and drift affect a navigation filter?<br>
**Approach:** a circular low-Earth orbit (r = 6771 km) is the truth trajectory. Random bits are converted to Gaussian noise (Box–Muller), added with a small drift to produce measurements, and a constant-velocity Kalman filter estimates the state; RMSE over time is plotted. Quantum-sourced bits come from a Qiskit Hadamard circuit or an optional public QRNG service.<br>
**Stack:** `Python` `Qiskit` `NumPy` `Streamlit` &nbsp;·&nbsp; **[Repository →](https://github.com/shrashtimittal/qrng-spacecraft-navigation)**<br>
<sub>Exploratory. Bits fall back to a classical generator if the quantum path is unavailable, no performance advantage is claimed, and it is not flight-validated navigation.</sub>

<br>

### HELIO-OPS Guardian System
<a href="https://github.com/shrashtimittal/HELIO-OPS-Guardian-System"><img src="assets/projects/helio.svg" width="100%" alt="Solar event rays and coronal mass ejection fronts reaching LEO, MEO and GEO satellite shells."></a>

**Question:** how can a solar event be translated into an interpretable operational risk for satellites in different orbits?<br>
**Approach:** an object-oriented model of solar events and satellites, with risk = magnitude × orbital exposure × (1 − shielding), a reduction for hardened spacecraft, and a safe-mode simulation with console dashboards.<br>
**Stack:** `Python` `Jupyter` &nbsp;·&nbsp; **[Repository →](https://github.com/shrashtimittal/HELIO-OPS-Guardian-System)**<br>
<sub>A conceptual prototype with a deliberately simplified model and generated scenarios. It does not use live space-weather data.</sub>

<br>

### Team Mimosa: Landsat 7 inspection mission study
<img src="assets/projects/mimosa.svg" width="100%" alt="An inspector spacecraft on a relative orbit around a Landsat 7 target above Earth's limb.">

**Question:** which real satellite is a suitable target for a free-flying inspector, and how does the inspection mission behave in simulation?<br>
**Approach:** a three-person SHE ORBITS 2026 team study: target-satellite selection supported by a decision-support workbook, then a GMAT simulation campaign and a design-status report.<br>
**Stack:** `GMAT` `Excel` &nbsp;·&nbsp; no public repository<br>
<sub>A summer-school concept study, not a flight programme; the reports are not public.</sub>

<br>

**More work**

| | |
|:--|:--|
| <img src="assets/projects/fraud.svg" width="140" alt="Fraud detection plate"> | **[Fraud Transaction Detection](https://github.com/shrashtimittal/fraud-transaction-detection)**<br>Logistic regression, random forest and XGBoost on simulated card transactions with class weighting. `scikit-learn` `XGBoost` |
| <img src="assets/projects/asl.svg" width="140" alt="ASL classes plate"> | **[ASL Sign Language Detection](https://github.com/shrashtimittal/asl-sign-language-detection)**<br>EfficientNet-B0 transfer learning on 29 classes, still images, Streamlit interface. `PyTorch` `timm` |
| <img src="assets/projects/animal.svg" width="140" alt="Animal classifier plate"> | **[Animal Image Classification](https://github.com/shrashtimittal/animal-image-classification)**<br>15-class EfficientNet-B0 classifier with a freeze-then-fine-tune schedule. `PyTorch` `timm` |
| <img src="assets/projects/finance.svg" width="140" alt="Finance manager plate"> | **[Personal Finance Manager](https://github.com/shrashtimittal/personal-finance-manager-cli)**<br>CLI-first Python application with SQLite, budgets, CSV export and an optional PySide6 GUI. |
| <img src="assets/projects/cubesat.svg" width="140" alt="CubeSat plate"> | **Smart CubeSat**<br>Satellite systems design project; public documentation to follow. |

<sub>No accuracy figures are quoted for the machine-learning projects because the repositories do not publish them.</sub>

<a name="robotics"></a>
<img src="assets/sections/robotics.svg" width="100%" alt="03 Robotics and embedded">

<img src="assets/icons/robotics.svg" width="36" alt="">

I work with flight-controller and microcontroller platforms for UAV and robotic systems, integrating sensors and writing embedded code in `C/C++` and `Python`.

| Layer | Platforms |
|:--|:--|
| Flight control | `Pixhawk` |
| Onboard computing | `Raspberry Pi` |
| Microcontrollers | `Arduino` `ESP32` `STM32` |
| Focus | Sensor integration, embedded development, autonomy |

<sub>Hardware project write-ups will be added here once documented for public release.</sub>

<a name="research"></a>
<img src="assets/sections/research.svg" width="100%" alt="04 Research">

**Themes:** astrophysics and dark matter &nbsp;·&nbsp; orbital and navigation concepts &nbsp;·&nbsp; quantum entanglement and theoretical physics &nbsp;·&nbsp; spacecraft systems and mission engineering.

Every entry is labelled with exactly one status: **published**, **conference presentation**, **submitted manuscript**, **ongoing independent research** or **exploratory theoretical work**. Nothing unpublished is presented as peer-reviewed, and no peer-reviewed publication is claimed on this page. Entries appear here with their abstract, PDF and DOI as they become public.

<a name="skills"></a>
<img src="assets/sections/skills.svg" width="100%" alt="05 Technical skills">

| Domain | Tools |
|:--|:--|
| **Programming and scientific computing** | `Python` `C/C++` `NumPy` `SciPy` `pandas` `Matplotlib` `Jupyter` |
| **Aerospace and mission simulation** | `GMAT` `Qiskit` Kalman filtering, Keplerian orbit simulation |
| **Robotics and embedded** | `Pixhawk` `Raspberry Pi` `Arduino` `ESP32` `STM32` |
| **AI and machine learning** | `PyTorch` `scikit-learn` `XGBoost` `timm` `OpenCV` |
| **Workflow** | `Git` `GitHub` `Streamlit` `SQLite` `pytest` |

<a name="activity"></a>
<img src="assets/sections/activity.svg" width="100%" alt="06 GitHub activity">

<div align="center">
<img src="assets/stats/repo-composition.svg" width="100%" alt="Source composition of the featured repositories: mostly Python, with Jupyter notebooks, QSS and SQL.">
</div>

<sub>A static snapshot of the featured repositories; live activity is on <a href="https://github.com/shrashtimittal">my GitHub profile</a>.</sub>

<a name="contact"></a>
<img src="assets/sections/contact.svg" width="100%" alt="07 Contact">

<table>
<tr>
<td width="72" valign="middle"><img src="assets/brand/monogram.svg" width="56" alt="SM monogram"></td>
<td valign="middle"><b>Shrashti Mittal</b><br>GitHub: <a href="https://github.com/shrashtimittal">github.com/shrashtimittal</a><br><sub>For research or engineering collaboration, open an issue or discussion on any repository above.</sub></td>
</tr>
</table>

<!-- Add after confirming what you want public:
LinkedIn: ...   Email: ...   ORCID: ...   Google Scholar: ...
-->

<div align="center">
<img src="assets/dividers/divider.svg" width="60%" alt="">
</div>
