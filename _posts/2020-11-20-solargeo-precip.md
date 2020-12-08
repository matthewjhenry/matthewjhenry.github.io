---
title: 'How does solar geoengineering affect precipitation?'
date: 2020-12-08
permalink: /posts/2020/11/solargeo-precip/
---

I would like to better understand how solar geoengineering might affect precipitation. Early climate model studies of solar geoengineering ([Robock et al. 2008](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2008JD010050) for example) showed that stratospheric aerosol injection could disrupt the Asian and African summer monsoons. However, the more recent solar geoengineering research shows that the climate outcome of stratospheric aerosol injection very much depends on the location, quantity, season, and type of reflectant used. The extent to which one can choose the climate outcome is still a topic of research.

## Radiative antidote to CO2

In ["Designing a radiative antidote to CO2"](https://www.essoar.org/pdfjs/10.1002/essoar.10504359.1), the authors ([Jake Seeley](https://www.jacobtseeley.com/), [Nick Lutsko](https://nicklutsko.github.io/), and [David Keith](https://keith.seas.harvard.edu/people/david-keith)) design an idealized reflectant that would perfectly offset the direct radiative effects of CO2. In their idealized climate model simulations, surface temperature *and* precipitation are kept to control values after increasing CO2 and reflecting solar radiation, by choosing the spectral bands within which shortwave radiation is attenuated.

## Their main result

They run radiative-convective simulations with the cloud-resolving model DAM (Romps, 2018). Their figure 4 below shows the surface temperature and precipitation change in their three main experiments. In red (4xCO2), they just quadruple CO2 concentrations, the surface temperature increases by 6.89K and precipitation increases by 18.4%. In blue (4xCO2 + USRM), they quadruple CO2 and apply a spectrally uniform reduction in insolation to keep the surface temperature constant. However, they end up with a 2.2% reduction in precipitation, which is consistent with the theory and comprehensive climate model simulations. In green (4xCO2 + SSRM), they quadruple CO2 and spectrally tune the reduction in insolation, such that the surface temperature *and* precipitation stay constant.

<br/>
<div style="text-align:center;valign:center"><img src="https://matthewjhenry.github.io/images/seeley_fig4.png" alt="" style="display: block; width: 800px; height: auto;"></div>
<br/>

## Tropospheric forcing leads to precipitation change

In an atmosphere in radiative-convective equilibrium, radiative cooling is balanced by the latent heat released in precipitating clouds. As shown in their equation 2, $\Delta P = -\alpha_P \Delta Q$, the change in precipitation ($\Delta P$) scales with the change in *tropospheric* radiative cooling. And tropospheric radiative cooling can be decomposed into a part directly affected by external perturbation (direct effect of CO2 for example) and a part that scales linearly with surface temperature change.

In the 4xCO2 case, surface temperature increases, which leads to an increase in tropospheric radiative cooling and hence an increase in precipitation. However, in both SRM experiments, the insolation is reduced such that the surface temperature change is zero, hence the only change in tropospheric radiative cooling comes from the direct effects of the forcings (CO2 and insolation).

Their figure 2 below shows the vertical profile of radiative forcing on the left and the decomposition into tropopause (TROP), atmospheric (ATM), and surface (SURF) forcings for each case. The tropopause forcing is the sum of the atmospheric and surface forcings, and the net forcing is the sum of the longwave and shortwave forcings. In the 4xCO2 case, the positive longwave forcing from increased CO2 at the tropopause comes from both the surface and atmosphere (approximately half each). The spectrally-uniform (USRM) reduction in insolation induces a negative tropospheric forcing that is proportional to the control shortwave atmospheric absorption, which is small. Hence the net atmospheric forcing is positive, which causes a reduction in precipitation (see equation above). In the spectrally tuned case (SSRM), the wavelengths are chosen such that the shortwave radiation is partially attenuated in the troposphere, which causes a negative forcing in the atmosphere, which balances the positive longwave forcing from CO2. Hence there is no change in precipitation.

<br/>
<div style="text-align:center;valign:center"><img src="https://matthewjhenry.github.io/images/seeley_fig2.png" alt="" style="display: block; width: 800px; height: auto;"></div>
<br/> 

## Use this to constrain changes in precipitation in the G1 GeoMIP experiments?

According to this theory, if the control atmosphere is more transparent to shortwave radiation, then the G1 experiment (4xCO2 + spectrally uniform reduction in insolation) should lead to a larger reduction in precipitation. I used some CMIP6 data to see if there is a correlation between the reduction in precipitation in G1 experiments (y-axis) and shortwave atmospheric absorption (x-axis). I actually use downwelling shortwave radiation at the surface in clear-sky conditions (from piControl simulations) as the TOA downwelling shortwave radiation should be the same for all models.

However, as shown below, there is no clear correlation between these two variables. Maybe I need more models to have a wider range of precipitation changes, or there is an error in my data processing, or my reasoning is too simplistic.

<br/>
<div style="text-align:center;valign:center"><img src="https://matthewjhenry.github.io/images/G1_precip_changes.png" alt="" style="display: block; width: 800px; height: auto;"></div>
<br/>

## Implications for real-world solar radiation management deployment

This theory is certainly relevant for the real-world because of the possibility of designing reflectants with the desired spectral attenuations. Moreover, the aerosols that are most commonly discussed (sulfate aerosols) do not lead to a spectrally uniform reduction in insolation, hence this theory helps us to understand how the deviation from spectral uniformity affects precipitation.