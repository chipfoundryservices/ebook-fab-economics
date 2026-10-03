# Chapter 3: Wafer Pricing Models, Die Cost & Yield Sensitivity

## 3.1 The Wafer ASP Escalation Curve
Leading-edge wafer pricing reflects the immense capital intensity of node transitions:
- $28\text{nm}$ Planar (2011): $\approx \$3,000$ per wafer
- $7\text{nm}$ FinFET (2018): $\approx \$10,000$ per wafer
- $5\text{nm}$ FinFET (2020): $\approx \$16,000$ per wafer
- $3\text{nm}$ FinFET (2023): $\approx \$20,000$ per wafer
- $2\text{nm}$ GAA Nanosheet (2025): $\approx \$25,000\text{–}\$30,000$ per wafer

## 3.2 Die Cost Economics: Good Die Formulation
The cost to a fabless customer per functional, tested die is governed by:

$$\text{Cost per Good Die} = \frac{\text{Wafer Cost}}{\text{Dies per Wafer} \times \text{Yield } Y}$$

Where the gross dies per $300\text{mm}$ wafer ($D = 300\text{mm}$) for a die of area $A$ is given by De Vries' formula:

$$\text{DPW} = \frac{\pi D^2}{4 A} - \frac{\pi D}{\sqrt{2 A}} = \frac{70,686}{A} - \frac{666}{\sqrt{A}}$$

For an $8.0\text{ cm}^2$ ($800\text{ mm}^2$) AI accelerator die:
- $\text{DPW} \approx 65\text{ dies/wafer}$
- At $50\%$ yield: $32.5$ good dies $\implies \text{Die Cost} = \$25,000 / 32.5 \approx \mathbf{\$769}$
- At $80\%$ yield: $52$ good dies $\implies \text{Die Cost} = \$25,000 / 52 \approx \mathbf{\$480}$

A $30\%$ improvement in yield saves the customer **$\$289$ per chip**, proving why fabless giants like Nvidia and Apple willingly pay a premium to fab exclusively at TSMC.
