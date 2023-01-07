# Time Series

This repo contains code I wrote to analyse and describe time series.

## time_series_asymptotic_properties_w_graphs.ipynb
I describe the asymptotic properties of the following time series:
* ### Stochastic Variable + Error Term
    * ### $x_t^{SV} = z + ε_t$
        - $ε_t∼i.i.d.(0,σ_{ε}^{2})$
        - $E(z) = 0$ , $Var(z) = σ_{z}^{2}$

* ### Moving Average Lag-1
    * ### $x_t^{MA(1)} = ε_t + θε_{t-1}$
        - $ε_t∼i.i.d.(0,σ_{ε}^{2})$
        - $0 < θ < 1$

* ### Disjoint sets of Random Variables with Breaks
    *  ### $x_t^{DRV} = μ_1 1_{\left(v_t ≤ γ \right)} + μ_2 1_{\left(v_t > γ \right)} + ɛ_t = μ_1 + δ 1_{\left(v_t > γ \right)}  + ɛ_t$
        - $δ = (μ_2 - μ_1)$
        - $ε_t∼i.i.d.(0,σ_{ε}^{2})$
        - $v_t∼i.i.d.(0,σ_{v}^{2})$
        - $𝐏(v_t > γ) = π$

* ### Time Series with Structural Break
    * ### $x_t^{TSB} = μ_1 1_{\left(t ≤ t^{\star} \right)} + μ_2 1_{\left(t > t^{\star} \right)} + ɛ_t = μ_1 + δ 1_{\left(t > t^{\star} \right)}  + ɛ_t$
        - $δ = (μ_2 - μ_1)$
        - $ε_t∼i.i.d.(0,σ_{ε}^{2})$

* ### Deterministic Trend with Constant and Error Term
    *  ### $x_t^{DT} = α + βt + ε_t$
        - $ε_t∼i.i.d.(0,σ_{ε}^{2})$

* ### Random Walk
    * ### $x_t^{RW} = x_{t-1} + ε_t = x_0 + ∑_{i=1}^{t} ε_i$
        - $ε_t∼i.i.d.(0,σ_{ε}^{2})$

* ### First-difference Random Walk
    * ### $d_1(t) = x_t^{RW} - x_{t-1}^{RW} = (x_{t-1} + ε_t) - x_{t-1} = ε_t$
        - $ε_t∼i.i.d.(0,σ_{ε}^{2})$
