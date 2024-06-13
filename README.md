# mplus_crosslevelint

## Author : 
* Jimin Kwon (Kyonggi Univ, Rep. of Korea)
* Jihyun Shin (Yonsei Univ, Rep. of Korea)

## Copyright
[MIT Lisence](LICENSE)

## Version info
### v0.5
This is a Mplus syntax for cross-level interaction between a L1 independent variable and L2 moderator, computed by creating random slopes in which each slope includes effects of an IV and L1 control variables on DV. These simple slopes are regressed onto a level 2 moderator for cross-level interaction analyses. Since this model does not distinguish random and fixed effect, it may have some methodological limitations as random slopes for cross-level interactions also include effects of control variables along with an effect of an independent variable. These limitations are to be further addressed in future release.

Mplus syntax for the analysis of a theoretical model that consists of one individual-level (L1) independent variable (X), two individuel-level dependent variables (Y1 & Y2), and one team-level (L2) moderator (W) that moderates the effects of X on Y1 and X on Y2.

## Script info
### DIRECTEFFECT_L1
Syntax for main effects of X on Y1 and X on Y2 along with a number of L1 control variables.
### MODERATOR_ON_DV
Multilevel syntax for effects of X and L1 control variables on Y1 and Y2, and also for effects of W and a L2 control variable on Y1 and Y2. This syntax was created solely to examine the effects of X, W, and control variables on Y1 and Y2 prior to the analysis of cross-level interaction between X and W on Y1 and Y2.
### CROSSLEVEL_INT
Multilevel syntax for a cross-level interaction between X and W on Y1 and Y2 by creating random slopes in which each slope includes effects of X and L1 control variables on Y1 and Y2, respectively. These random slopes are then regressed onto a level 2 moderator for cross-level interaction analyses. Note that in creating these random slopes, effects of L1 control variables are included such that for example, S1 was defined as Y1 on X L1CTRL1 L1CTRL2 L1CTRL3. Thus, fixed effects of Y1 on L1CTRL1 L1CTRL2 L1CTRL3 were examined in a separate model (MODERATOR_ON_DV syntax). This was specifically done as the original dataset has shown statistically significant difference in effects of control variables across clusters (teams), which motivated us to include these fixed effects for S1 and S2. Results may vary for any other datasets other than the one that this syntax was based on.

## REFERENCES
1. Muthen & Muthen (2017)
2. Bauer & Curran (2005) 
3. Hofmann & Gavin (1998)
4. Stride, Gardner, Catley, Thomas (2015)
