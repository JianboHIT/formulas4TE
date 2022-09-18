### P003: Device Figure-of-Merit (ZTdev) (G.J. Snyder et al., 2017)

> &bull; G.J. Snyder, A.H. Snyder, Figure of merit zt of a thermoelectric device defined from materials properties, Energy Environ. Sci. 10 (11) (2017) 2280-2283. [https://doi.org/10.1039/C7EE02007D](https://doi.org/10.1039/C7EE02007D).
> 

$$ $$

$$ +------------------------------------------+ $$

$$ (ZT)\_{dev} = \left[ \frac{T\_{h} - T\_{c}(1-\eta)}{T\_{h}(1-\eta) - T\_{c}} \right] ^{2} - 1 $$

$$ +------------------------------------------+ $$

$$ \eta = 1 - \frac{\Phi(T\_{c})}{\Phi(T\_{h})} $$

$$ \Phi = ST+1/u $$

$$ \frac{1}{u\_{n}} = \frac{1}{u\_{n-1}} \sqrt{1 - u\_{n-1}^2 (\rho _{n} \kappa _{n} + \rho _{n-1} \kappa _{n-1})(T\_{n} - T\_{n-1})} - \left( \frac{T\_{n} + T\_{n-1}}{2} \right) (S\_{n} - S\_{n-1}) $$

$$ +------------------------------------------+ $$

--------------------------------------------------

***An Explanation*** :

*&bull; Ref: G. J. Snyder, Thermoelectric Power Generation: Efficiency and Compatibility, in Thermoelectrics Handbook: Macro to Nano, ed. D. M. Rowe, CRC Press, 2006, ch. 9.*

The steady-state heat equation is given as 

$$ \nabla (\kappa \nabla T) = - T \frac{dS}{dT} J \nabla T - \rho J^2 $$

Consider the relative (reduced) current density *u*, which is defined as 

$$ u = \frac{J}{\nabla T} $$

we can rewirte the steady-state heat equation as 

$$ \frac{du}{dT} = u^{2} T \frac{dS}{dT} + u^{3} \rho \kappa $$

also as 

$$ \frac{d}{dT} \left( \frac{1}{u^{2}} \right) = -2 \left( \frac{T}{u} \frac{dS}{dT} + \rho \kappa \right) $$

For computation, it can be approximated by 

$$ \frac{1}{u\_{n}^2} - \frac{1}{u\_{n-1}^2} = -2 (T\_{n} - T\_{n-1}) \left( \frac{T\_{n} + T\_{n-1}}{2} \frac{1}{u\_{n}} \frac{S\_{n} - S\_{n-1}}{T\_{n} - T\_{n-1}} + \frac{\rho _{n} \kappa _{n} + \rho _{n-1} \kappa _{n-1}}{2} \right) $$

$$ \frac{1}{u\_{n}^2} + \frac{1}{u\_{n}} (T\_{n} + T\_{n-1}) (S\_{n} - S\_{n-1}) = \frac{1}{u\_{n-1}^2} -(T\_{n} - T\_{n-1}) (\rho _{n} \kappa _{n} + \rho _{n-1} \kappa _{n-1}) $$

$$ \left[ \frac{1}{u\_{n}} +  \left( \frac{T\_{n} + T\_{n-1}}{2} \right) (S\_{n} - S\_{n-1}) \right] ^2 = \frac{1}{u\_{n-1}^2} -(T\_{n} - T\_{n-1}) (\rho _{n} \kappa _{n} + \rho _{n-1} \kappa _{n-1}) + \left[ \left( \frac{T\_{n} + T\_{n-1}}{2} \right) (S\_{n} - S\_{n-1}) \right] ^2 $$

$$ \frac{1}{u\_{n}} +  \left( \frac{T\_{n} + T\_{n-1}}{2} \right) (S\_{n} - S\_{n-1}) \cong \sqrt{\frac{1}{u\_{n-1}^2} -(T\_{n} - T\_{n-1}) (\rho _{n} \kappa _{n} + \rho _{n-1} \kappa _{n-1})} $$

$$ \frac{1}{u\_{n}} = \frac{1}{u\_{n-1}} \sqrt{1 - u\_{n-1}^2 (\rho _{n} \kappa _{n} + \rho _{n-1} \kappa _{n-1})(T\_{n} - T\_{n-1})} - \left( \frac{T\_{n} + T\_{n-1}}{2} \right) (S\_{n} - S\_{n-1}) $$

When a trial *u* is given, we can slove the steady-state heat equation and calculate the efficiency $\eta$ of a thermoelectric device by thermoelectric potential $\Phi$, 

$$ \eta = 1 - \frac{\Phi(T\_{c})}{\Phi(T\_{h})} $$

$$ \Phi = ST+1/u $$

As the value of u is optimized, the efficiency will reach the maximum.


