# Ordinary Differential Equations in Vision and Language

Ordinary differential equations (ODEs) and related differential-equation formalisms are powerful mathematical tools for modeling a wide range of deep learning problems. In essence, an ODE describes how the state of a system changes as time varies. Here “time” can mean physical time, network depth, or a noise level used in generative modeling. A canonical form is

$$\frac{d\mathbf{x}(t)}{dt}=f(\mathbf{x}(t),t),$$

where $\mathbf{x}(t)$ denotes the evolving state (e.g., features or latent variables) and $f$ specifies the rule that drives its evolution. Depending on how we choose the state $\mathbf{x}(t)$, the dynamics $f$, and the notion of time $t$, this template naturally connects to many modern learning frameworks: residual networks can be interpreted as discrete-time approximations of an underlying continuous evolution, neural ODEs treat depth as a continuous variable and model the transformation as a continuous trajectory, and diffusion models in both vision and language can be viewed as time-indexed processes that progressively transform noise into data. Framed this way, ODEs provide a unified language for analyzing how information flows through a model and how inputs map to outputs—covering concrete applications such as image generation with diffusion/score-based models and mask-predict language models that generate text by iteratively denoising masked tokens over time.


