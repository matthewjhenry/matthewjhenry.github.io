---
layout: post
title: "Fun with FaIR: How many years of temporarily reduced emissions (such as a pandemic!) does it take to make a dent in the 2100 temperature projection?"
date: 2020-04-30
use_math: true
---

I played with <a href='https://fair.readthedocs.io/'>FaIR</a> $($Finite Amplitude Impulse Response simple climate model$)$ to look at the impact of the temporary reduction in emissions on global mean surface temperature change. The projected decrease in greenhouse gas emissions as a result of the pandemic vary a lot, but I just wanted to play with this model and have a sense of orders of magnitude.

The total temperature change from increased CO2 is a function of cumulative emissions so it is no surprise that a temporary reduction in emissions does not change the temperature at 2100 that much. But just how long does it take to make a dent?

I made a few simple assumptions to get an upper bound on temperature change: we follow RCP4.5 and years of "reduced" emissions actually have zero$($!$)$ emissions.

For 2 years of zero emissions, we barely get any change in temperature at 2100.

<div style="text-align:center;valign:center"><img src="https://matthewjhenry.github.io/images/Fair2.png" alt="" style="width: 700px; height: auto;"></div>

For 10 years of zero emissions, we get order 0.1 degrees less warming by 2100.

<div style="text-align:center;valign:center"><img src="https://matthewjhenry.github.io/images/Fair10.png" alt="" style="width: 700px; height: auto;"></div>

Finally, for 30 years of zero emissions, we get order 0.5 degrees less warming by 2100.

<div style="text-align:center;valign:center"><img src="https://matthewjhenry.github.io/images/Fair30.png" alt="" style="width: 700px; height: auto;"></div>

Check out the $($barely modified tutorial$)$ code <a href="https://matthewjhenry.github.io/code/FunFaIR.ipynb">here</a>.

