# Appendix B: Mathematical Derivations

## B.1 De Vries Gross Dies per Wafer (DPW) Derivation
Consider a circular wafer of diameter $D$ (radius $R = D/2$) upon which rectangular dies of width $w$ and height $h$ (die area $A = w \cdot h$) are fabricated.

The total wafer surface area is:

$$A_{\text{wafer}} = \pi R^2 = \frac{\pi D^2}{4}$$

To first order, the gross number of dies is $A_{\text{wafer}} / A$. However, dies intersecting the circular wafer perimeter cannot be completed.
The perimeter of the wafer is $P = \pi D$. The width of the dead exclusion zone around the boundary is approximately the average diagonal projection of a die:

$$\Delta r \approx \frac{\sqrt{w^2 + h^2}}{2} \approx \sqrt{\frac{A}{2}}$$

The area lost to edge-exclusion is:

$$A_{\text{lost}} \approx P \cdot \Delta r = \pi D \sqrt{\frac{A}{2}} = \frac{\pi D \sqrt{A}}{\sqrt{2}}$$

Dividing the usable area by die area $A$:

$$\text{DPW} = \frac{A_{\text{wafer}} - A_{\text{lost}}}{A} = \frac{\pi D^2}{4 A} - \frac{\pi D}{\sqrt{2 A}}$$

For a standard $300\text{mm}$ wafer ($D = 300\text{ mm}$):

$$\text{DPW} = \frac{\pi (300)^2}{4 A} - \frac{\pi (300)}{\sqrt{2 A}} = \frac{70,686}{A} - \frac{666}{\sqrt{A}} \quad (A \text{ in } \text{mm}^2)$$

## B.2 Operating Leverage Elasticity Formulation
Let $R$ be total revenue, $P$ be wafer ASP, $Q$ be wafer volume, $F$ be fixed costs (depreciation, plant overhead), and $v$ be variable cost per wafer:

$$\text{Operating Profit } \Pi = Q(P - v) - F$$

The Degree of Operating Leverage (DOL) at output level $Q$ is defined as the elasticity of operating profit with respect to wafer output:

$$\text{DOL} \equiv \frac{\% \Delta \Pi}{\% \Delta Q} = \frac{Q}{\Pi} \frac{d\Pi}{dQ} = \frac{Q (P - v)}{Q(P - v) - F} = \frac{\text{Contribution Margin}}{\text{Operating Profit}}$$

When a fab operates near breakeven ($\Pi \to 0$):

$$\text{DOL} \to \infty$$

A tiny $2\%$ surge in wafer volume creates a $100\%+$ increase in operating profit, mathematically proving why foundries fiercely protect capacity utilization above $90\%$.
