# formulas4TE

<!-- block::start::motivation -->

***Summary some formulas and equations for thermoelectricity(TE)***

> Read this in other languages: [简体中文](README.md), English

&nbsp;&nbsp;&nbsp;&nbsp;We often need to use some formulas repeatedly in thermoelectric research. 
Although, an efficient built-in equation editor is embedded in MicroSoft Office, 
it still takes some time to edit these numerous complex repetitive formulas. 
Here, some frequently used and reported formulas are collected, which not only facilitates the use of screenshots, 
but also can be easily copied to MicroSoft Office as an embedded equation (see 
**[Appendix: How to use equations in MicroSoft Office](#appendix-how-to-use-equations-in-microsoft-office)**
), improving work efficiency. Any bug reports or suggestions are very welcome, which can be discussed at 
[Issues](../../issues) page.

<!-- block::end::motivation -->

- [Basic Principles](#basic-principles)
- [APS-SPB Model](#aps-spb-model)
- [APS-SKB model](#aps-skb-model)
- [Boltzmann Equation Description of Electron Transport](#boltzmann-equation-description-of-electron-transport)
- [Expressions for Multiband Conduction](#expressions-for-multiband-conduction)
- [Equations in Papers](#equations-in-papers)
  - [P001: Engineering Thermoelectric Model (ZTeng) (H.S. Kim et al., 2015)](#p001-engineering-thermoelectric-model-zteng-hs-kim-et-al-2015)
  - [P002: Restructure SPB (RSPB) Model (J. Zhu et al., 2021)](#p002-restructure-spb-rspb-model-j-zhu-et-al-2021)
  - [P003: Device Figure-of-Merit (ZTdev) (G.J. Snyder et al., 2017)](#p003-device-figure-of-merit-ztdev-gj-snyder-et-al-2017)

<!-- block::start::content-zh --> 

- **[Appendix: How to use equations in MicroSoft Office](#appendix-how-to-use-equations-in-microsoft-office)**
    - [Method 1 (Both MicroSoft Word and PPT support)](#-method-1-both-microsoft-word-and-ppt-support)
    - [Method 2 (Only Word supports)](#-method-2-only-word-supports)

<!-- block::end::content-zh -->


## Basic Principles

$$ZT=\frac{\sigma S^2}{\kappa} \cdot T$$

$$PF=\sigma S^{2}$$

$$\sigma = ne\mu$$

$$ \mu = e \frac{\tau}{m^{\ast}} $$

$$\kappa = \kappa_{L} + \kappa_{e} + \kappa_{bip} $$

$$\kappa_{L} = \frac{1}{3} C_{v}vl$$

$$\kappa_{e} = L \sigma T$$

$$\eta = \frac{T_{h}-T_{c}}{T_{h}} \cdot \frac{\sqrt{1+ZT}-1}{\sqrt{1+ZT}+T_{c} / T_{h}}$$

$$s = \frac{\sqrt{1+ZT}-1}{S \cdot T}$$

$$ \beta = \frac{\mu_{0} (m^{\ast}/m_{e})^{3/2} T^{3/2}}{\kappa_{L}}T $$


## APS-SPB Model

*Single parabolic band (SPB) model with acoustic phonon scattering (APS) mechanism and deformation potential theory*

$$ E = \frac{\hbar ^{2} k^{2}}{2 m^{\ast}} $$

$$ g(E) = \frac{(2 m_{d} ^{\ast})^{3/2}}{2 \pi^{2} \hbar^{3}} E^{1/2} = \frac{N_{v} (2 m_{b} ^{\ast})^{3/2}}{2 \pi^{2} \hbar^{3}} E^{1/2} $$

$$ v^{2}(E) = \frac{2E}{m_{b} ^{\ast}} $$

$$ \tau(E) = \frac{N_{v} \hbar C_{ii}}{\pi  k_{B} T {\Xi ^{2}}} \frac{1}{g(E)} = \frac{2 \pi \hbar^{4} C_{ii}}{(2 m_{b} ^{\ast})^{3/2} k_{B} T {\Xi ^{2}}} E^{-1/2} $$

$$ F_{n}(\eta) = \int _{0}^{+\infty} {{\frac{x^{n}}{1+\exp (x-\eta)}}} dx $$

$$ x = \frac{E}{k_{B}T}, \eta = \frac{E_{F}}{k_{B}T} $$

$$ n = \frac{N_{v}( 2 m_{b} ^{\ast} k_{B} T )^{3/2}}{2\pi ^{2} \hbar ^{3}} F_{1/2}( \eta ) $$

$$ \mu = \frac{4 \pi e \hbar ^{4} C_{ii}}{m_{I} ^{\ast} (2 m_{b} ^{\ast} k_{B} T)^{3/2} \Xi ^{2}} \frac{F_{0}(\eta)}{3 F_{1/2}(\eta)} $$

$$ \sigma = \frac{2 N_{v} e^2 \hbar C_{ii}}{3 \pi m_{I} ^{\ast} \Xi ^{2} } F_{0}(\eta)$$

$$ S = \frac{k_{B}}{e} \left( \frac{2 F_{1}(\eta)}{F_{0}(\eta)} - \eta \right) $$

$$ L = \frac{k_{B}^{2}}{e^{2}} \left[ 3 \frac{F_{2}(\eta)}{F_{0}(\eta)} - 4 \left( \frac{F_{1}(\eta) }{F_{0}(\eta)} \right) ^{2} \right] $$

$$ r_{H} = \frac{n}{n_{H}} = \frac{\mu_{H}}{\mu} = \frac{3 F_{1/2}(\eta) F_{-1/2}(\eta)}{4 F_{0}^{2}(\eta)} $$


## APS-SKB model

*Single Kane band (SKB) model with acoustic phonon scattering (APS) mechanism and deformation potential theory*

$$ E \left( 1+\frac{E}{E_{g}} \right) = \frac{\hbar ^{2} k^{2}}{2 m^{\ast}} $$

$$ g(E) = \frac{N_{v} (2 m_{b} ^{\ast})^{3/2}}{2 \pi^{2} \hbar^{3}} E^{1/2} \left( 1+\frac{E}{E_{g}} \right) ^{1/2} \left( 1 + 2 \frac{E}{E_{g}} \right) $$

$$ v^{2}(E) = \frac{2E}{m_{b} ^{\ast}} \left( 1+\frac{E}{E_{g}} \right) \left( 1 + 2 \frac{E}{E_{g}} \right) ^{-2} $$

$$ \tau(E) = \frac{N_{v} \hbar C_{ii}}{\pi  k_{B} T \Xi ^{2}} \frac{1}{g(E)} \frac{3(1+2E/E_{g})^{2}}{(1+2E/E_{g})^{2}+2} $$

$$ F^{n}_{m,k}(\eta, \alpha) = \int _{0}^{+\infty}{x^{n} (x+\alpha x^{2})^{m}[(1+2\alpha x)^{2} + 2]^{k/2} \left( -\frac{\partial f}{\partial x} \right)}dx $$

$$ x = \frac{E}{k_{B}T}, \eta = \frac{E_{F}}{k_{B}T}, \alpha = \frac{k_{B}T}{E_{g}} $$

$$ n = \frac{N_{v}( 2 m_{b} ^{\ast} k_{B} T )^{3/2}}{3\pi ^{2} \hbar ^{3}} {F^{0}_{3/2,0}(\eta, \alpha)} $$

$$ \mu = \frac{2 \pi e \hbar ^{4} C_{ii}}{m_{I} ^{\ast} (2 m_{b} ^{\ast} k_{B} T)^{3/2} \Xi ^{2}} \frac{3 F^{0} _{1,-2}(\eta, \alpha)}{F^{0} _{3/2,0}(\eta, \alpha)} $$

$$ \sigma = \frac{2 N_{v} e^{2} \hbar C_{ii}}{\pi m_{I} ^{\ast} \Xi ^{2} }{F^{0} _{1,-2}(\eta, \alpha)} $$

$$ S = \frac{k_{B}}{e} \left( \frac{F^{1} _{1,-2}(\eta, \alpha)}{F^{0} _{1,-2}(\eta, \alpha)} - \eta \right) $$

$$ L = \frac{k_{B}^{2}}{e^{2}} \left[ \frac{F^{2} _{1,-2}(\eta, \alpha)}{F^{0} _{1,-2}(\eta, \alpha)} - \left( \frac{F^{1} _{1,-2}(\eta, \alpha)}{F^{0} _{1,-2}(\eta, \alpha)} \right) ^{2} \right] $$

$$ r_{H} = \frac{n}{n_{H}} = \frac{\mu_{H}}{\mu} = \frac{{F^{0} _{3/2,0}(\eta, \alpha)}\cdot {F^{0} _{1/2,-4}(\eta, \alpha)}}{\left( {F^{0} _{1,-2}(\eta, \alpha)} \right) ^{2}} $$


## Boltzmann Equation Description of Electron Transport

$$ f = \frac{1}{1+\exp \left( \frac{E - E_{F}}{k_{B} T} \right)} $$

$$ n = \int_{0}^{+\infty} {f \cdot g(E)} dE $$

$$ p = \int_{-\infty}^{0} {(1-f) \cdot g(E)} dE $$

$$ \sigma(E) = e^2 \tau(E)v^{2}(E)g(E) $$

$$ \sigma = \int_{-\infty}^{+\infty}{\sigma(E) \cdot \left( -\frac{\partial f}{\partial E} \right)} dE $$

$$ S = -\frac{1}{\sigma \cdot eT} \int_{-\infty}^{+\infty}{\sigma(E) \cdot (E-E_{F})\left( -\frac{\partial f}{\partial E} \right)} dE $$

$$ \kappa_{e} = \frac{1}{e^{2}T} \int_{-\infty}^{+\infty}{\sigma(E) \cdot (E-E_{F})^{2} \left( -\frac{\partial f}{\partial E} \right)} dE - \sigma S^{2} T $$


## Expressions for Multiband Conduction

$$ n = \sum_{i}{n_{i}} $$

$$ \sigma = \sum_{i} {\sigma_{i}} $$

$$ S = \frac{\sum_{i}{\sigma_{i} S_{i}}}{\sum_{i}{\sigma_{i}}} $$

$$ R_{H} = \frac{\sum_{i}{\sigma_{i}^{2} R_{H,i}}}{\left( \sum_{i}{\sigma_{i}} \right) ^{2}} $$

$$ \kappa_{e} = \left[ {\sum_{i}{L_{i} \sigma_{i}} + \sum_{i}{\sigma_{i} S_{i}^{2}} - \frac{\left( \sum_{i}{\sigma_{i} S_{i}} \right) ^{2}}{\sum_{i}{\sigma_{i}}} } \right] \cdot T $$


## Equations in Papers

### P001: Engineering Thermoelectric Model (ZTeng) (H.S. Kim et al., 2015)

$$ \eta_{max} = \eta _{c} \frac{\sqrt{1 + (ZT) _{eng} \alpha _{1} \eta _{c}^{-1}} - 1}{\alpha _{0} \sqrt{1 + (ZT) _{eng} \alpha _{1} \eta _c^{-1}} + \alpha _{2}} $$

([Return &#8673;](#formulas4te) | [Show Details ...](papers/P001.md))

> &bull; H.S. Kim, W. Liu, G. Chen, C. Chu, Z. Ren, Relationship between thermoelectric figure of merit and energy conversion efficiency, Proceedings of the National Academy of Sciences 112 (27) (2015) 8205-8210. [ https://doi.org/10.1073/pnas.1510231112](https://doi.org/10.1073/pnas.1510231112)

### P002: Restructure SPB (RSPB) Model (J. Zhu et al., 2021)

$$ S_{r} = \ln \left( 1.075 + \frac{e^{2}}{n_{r}} \right) $$

([Return &#8673;](#formulas4te) | [Show Details ...](papers/P002.md))

> &bull; J. Zhu, X. Zhang, M. Guo, J. Li, J. Hu, S. Cai, W. Cai, Y. Zhang, J. Sui, Restructured single parabolic band model for quick analysis in thermoelectricity, npj computational materials 7 (1) (2021) 1-8. [https://doi.org/10.1038/s41524-021-00587-5](https://doi.org/10.1038/s41524-021-00587-5)
>
> &bull; GitHub rSPB respository. [https://github.com/JianboHIT/rSPB](https://github.com/JianboHIT/rSPB)

### P003: Device Figure-of-Merit (ZTdev) (G.J. Snyder et al., 2017)

$$ (ZT)\_{dev} = \left[ \frac{T\_{h} - T\_{c}(1-\eta)}{T\_{h}(1-\eta) - T\_{c}} \right] ^{2} - 1 $$

([Return &#8673;](#formulas4te) | [Show Details ...](papers/P003.md))

> &bull; G.J. Snyder, A.H. Snyder, Figure of merit zt of a thermoelectric device defined from materials properties, Energy Environ. Sci. 10 (11) (2017) 2280-2283. [https://doi.org/10.1039/C7EE02007D](https://doi.org/10.1039/C7EE02007D).

<!-- block::start::howto -->

## Appendix: How to use equations in MicroSoft Office

### &bull; Method 1 (Both MicroSoft Word and PPT support)

1. Right click on the equation, select **Copy to Clipboard** > **TeX Commands**.

<img src="pictures/step-1-1.png" width="85%">

2. Select **Insert** > **Equation** or press `Alt + =` in **Word** or **PPT**.

<img src="pictures/step-1-2.png" width="85%">

3. Click `{}LaTeX` to enable LaTeX mode in the **Equation** ribbon.

<img src="pictures/step-1-3.png" width="85%">

4. Paste (`Ctrl + V`) and press `Enter`.

<img src="pictures/step-1-4.png" width="85%">

5. Done.

<img src="pictures/step-1-5.png" width="85%">

### &bull; Method 2 (Only Word supports)

1. Right click on the equation, select **Copy to Clipboard** > **MathML Code**.

<img src="pictures/step-2-1.png" width="85%">

2. Paste (`Ctrl + V`) in Word.

<img src="pictures/step-2-2.png" width="85%">

3. Done.

<img src="pictures/step-2-3.png" width="85%">

<!-- block::end::howto -->
