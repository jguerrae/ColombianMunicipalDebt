# Staying in Power: Political Continuity and Local Fiscal Outcomes in Colombia

## Authors
[Jaime Bonet-Morón](https://investiga.banrep.gov.co/es/profile/73), [Jhorland Ayala-García](https://investiga.banrep.gov.co/es/profile/75), Jorge Guerra-España

## Description
This research examines the causal impact of political continuity on local debt levels, employing a sophisticated empirical strategy to address the intrinsic challenges of measuring political effects on municipal finances. The focus is on understanding how re-election strategies that target public spending may non-randomly affect election outcomes.

### Empirical Strategy and Data
The study uses a regression kink design (RKD) to investigate the subtle dynamics between political continuity and fiscal outcomes, specifically the role of local debt. This method extends the traditional regression discontinuity design (RDD), capturing not just shifts in policy application but variations in their intensity.

#### Methodology
RKD is deployed to explore how policy changes at known thresholds—like the margin of vote victory or loss—affect debt levels. The treatment variable \( T \) is defined based on the election outcome:
\[ T(V) = \begin{cases} 
0 & \text{if } V < v_0 \\
1 & \text{if } V \geq v_0 
\end{cases} \]
where \( V \) is the vote margin, and \( v_0 \) is the threshold (set at zero), distinguishing between winners and losers. The primary interest is the treatment effect on the debt level \( Y \), particularly the change in slope of the debt function at the threshold:
\[ E[y_1(1,0,U) | V = v_0] = \lim_{v_0 \to 0^+} \frac{dE[Y | V = v]}{dv}\bigg|_{v=v_0} - \lim_{v_0 \to 0^-} \frac{dE[Y | V = v]}{dv}\bigg|_{v=v_0} \]

#### Estimation Technique
The estimation approach involves specifying a model where the outcome \( Y_i \) of municipal debt is modeled as:
\[ Y_i = \alpha + \tau T_i + f(v_i) + U_i \quad \forall v_i \in (v_0 - h, v_0 + h) \]
The function \( f(v_i) \) is adjusted to capture the local variations and is typically a polynomial function:
\[ f(v_i) = \beta v_i + \phi T_i v_i \]
This specification allows for an examination of the differential impact of being elected on the slope of the debt function across the vote margin threshold.

### Conclusions and Implications
The findings suggest that political continuity, as manifested through repeated election victories, significantly impacts local debt levels, emphasizing the nuanced effects of political incentives on fiscal outcomes. This analysis contributes to understanding the fiscal behaviors influenced by political cycles in Colombian municipalities.

## License
This project is licensed under the MIT License, allowing its use, modification, and distribution under certain conditions.

### Contact
For questions or collaborations, please contact [Jorge Guerra](mailto:ja.guerrae@uniandes.edu.co)
