# formulas4TE(under-developed)
Summary some formulas and equations for thermoelectricity(TE)

> 选择语言：简体中文, English(*TODO*)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在热电研究中，我们常常需要反复地使用一些公式。
尽管目前 MicroSoft Office 提供了非常方便的内嵌公式编辑器，但是由于公式的形式较为复杂，
因此我们还是需要花费大量的时间来输入这些公式。这里，我们总结了一些高频使用的公式，
不但能够方便截图使用，同时也能够非常容易地粘贴为 MicroSoft Office 的内嵌公式
（参考后面的**附录：如何在 MicroSoft Office 中使用这里的公式**），提高工作效率。

<!--

### Preview version

$$ZT=\frac{\sigma S^2}{\kappa} \cdot T$$

$$PF=\sigma S^{2}$$

$$\sigma = ne\mu$$

$$\kappa = \kappa_{L} + \kappa_{e} + \kappa_{bip} $$

$$\eta = \frac{T_{h}-T_{c}}{T_{h}} \cdot \frac{\sqrt{1+ZT}-1}{\sqrt{1+ZT}+T_{c} / T_{h}}$$

$$s = \frac{\sqrt{1+ZT}-1}{S \cdot T}$$

$$ZT_{dev} = \left[{ \frac{T_{h}-T_{c}(1-\eta)}{T_{h}(1-\eta)-T_{c}}}\right]^{2}-1$$

$$S_{r} = \ln \left( {1.075 + \frac{e^{2}}{n_{r}}} \right)$$

$$\mu_{r} = \left( {1 + \frac{n_{r}}{2}} \right)^{-1/3}$$

$$L_{r} = 2 + \frac{\pi^{2}/3-2}{\left[ {1+(n_{r}/2\pi)^{-3/2}} \right] ^ {3/2}}$$

-->

## Basic Principles

$$ZT=\frac{\sigma S^2}{\kappa} \cdot T$$

$$PF=\sigma S^{2}$$

$$\sigma = ne\mu$$

$$\mu = e \frac{\tau}{m^{*}}$$

$$\kappa = \kappa_{L} + \kappa_{e} + \kappa_{bip} $$

$$\kappa_{L} = \frac{1}{3} \cdot C_{v}vl$$

$$\kappa_{e} = L \sigma T$$

$$\eta = \frac{T_{h}-T_{c}}{T_{h}} \cdot \frac{\sqrt{1+ZT}-1}{\sqrt{1+ZT}+T_{c} / T_{h}}$$

$$s = \frac{\sqrt{1+ZT}-1}{S \cdot T}$$

$$ \beta = \frac{\mu_{0} (m^{*}/m_{e})^{3/2} T^{3/2}}{\kappa_{L}}T $$


## APS-SPB Model

*Single parabolic band (SPB) model with acoustic phonon scattering (APS) mechanism and deformation potential theory*

$$ E = \frac{\hbar ^{2} k^{2}}{2 m^{*}} $$

$$ g(E) = \frac{(2 m_{d}^{*})^{3/2}}{2 \pi^{2} \hbar^{3}} E^{1/2} = \frac{N_{v} (2 m_{b}^{*})^{3/2}}{2 \pi^{2} \hbar^{3}} E^{1/2} $$

$$ \tau = \frac{N_{v} \hbar C_{ii}}{\pi  k_{B} T \Xi ^{2}} \frac{1}{g(E)} = \frac{2 \pi \hbar^{4} C_{ii}}{(2 m^{*})^{3/2} k_{B} T \Xi^{2}} E^{-1/2} $$

$$ F_{n}(\eta) = \int_{0}^{+\infty} \frac{x^{n}}{1+\exp (x-\eta)} dx $$

$$ n = \frac{N_{v}( 2 m_{b}^{*} k_{B} T )^{3/2}}{2\pi ^{2} \hbar ^{3}} F_{1/2}( \eta ) $$

$$ \mu = \frac{4 \pi e \hbar ^{4} C_{ii}}{m_{I}^{*} (2 m_{b}^{*} k_{B} T)^{3/2} \Xi ^{2}} \frac{F_{0}(\eta)}{3 F_{1/2}(\eta)} $$

$$ \sigma = \frac{2 N_{v} e^2 \hbar C_{ii}}{3 \pi m_{I}^{*} \Xi ^{2} } F_{0}(\eta)$$

$$ S = \frac{k_{B}}{e} \left( \frac{2 F_{1}(\eta)}{F_{0}(\eta)} - \eta \right) $$

$$ L = \frac{k_{B}^{2}}{e^{2}} \frac{3 F_{0}(\eta) F_{2}(\eta) - 4 F_{1}^{2}(\eta) }{F_{0}^{2}(\eta)} $$

$$ r_{H} = \frac{n}{n_{H}} = \frac{\mu_{H}}{\mu} = \frac{3 F_{1/2}(\eta) F_{-1/2}(\eta)}{4 F_{0}^{2}(\eta)} $$


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


## 附录：如何在 MicroSoft Office 中使用这里的公式

### &bull; 方法一（适用于 Word 和 PPT）

1. 在网页中的公式上右键，点击 **Copy to Clipboard** > **TeX Commands**；

<img src="pictures/step-1-1.png" width="85%">

2. 在 **Word** 或者 **PPT** 中，点击 **插入** > **方程**，或者使用快捷键 `Alt + =`；

<img src="pictures/step-1-2.png" width="85%">

3. 在 **公式** 选项卡中点击 `{}LaTeX` ，切换为 LaTeX 输入模式；

<img src="pictures/step-1-3.png" width="85%">

4. 粘贴内容（快捷键 `Ctrl + V`），然后按回车（`Enter`）键；

<img src="pictures/step-1-4.png" width="85%">

5. 完成。

<img src="pictures/step-1-5.png" width="85%">

### &bull; 方法二（仅适用于 Word）

1. 在网页中的公式上右键，点击 **Copy to Clipboard** > **MathML Code**；

<img src="pictures/step-2-1.png" width="85%">

2. 在 **Word** 中直接粘贴（快捷键 `Ctrl + V`）；

<img src="pictures/step-2-2.png" width="85%">

3. 完成。

<img src="pictures/step-2-3.png" width="85%">
