# Ordinary Differential Equations in Vision and Language

Ordinary differential equations (ODEs) and related differential-equation formalisms are powerful mathematical tools for modeling a wide range of deep learning problems. In essence, an ODE describes how the state of a system changes as time varies. Here "time" can represent physical time, network depth, or the noise level used in generative modeling. The canonical form of an ODE is

$$\frac{d\mathbf{x}(t)}{dt}=f(\mathbf{x}(t),t),$$

where $\mathbf{x}(t)$ denotes the evolving state (e.g., features or latent variables) and $f$ specifies the rule driving its evolution. Depending on the choice of state $\mathbf{x}(t)$, dynamics $f$, and the notion of time $t$, this template naturally connects to many modern learning frameworks: residual networks can be interpreted as discrete-time approximations of an underlying continuous evolution, neural ODEs treat depth as a continuous variable and model the transformation as a continuous trajectory, and diffusion models in both vision and language can be viewed as time-indexed processes that progressively transform noise into data. Framed this way, ODEs provide a unified language for analyzing how information flows through a model and how inputs map to outputs. Thus they can cover many applications in AI, such as image generation with diffusion models and mask-predict language models that generate text by iteratively denoising masked tokens over time.

In the article ***Ordinary Differential Equations in Vision and Language***, we explore how ODEs inspire and construct advanced AI models through three progressive levels: First, we interpret classic residual networks and their variants as direct discretizations of ODEs, examining how this perspective guides the design of architectures such as Transformers. Second, we introduce neural ODEs based on fully continuous-time modeling and their applications in flows. Finally, we discuss diffusion models as a connection between discrete and continuous frameworks. We outline how they model generation processes in vision and language from the perspective of differential equations.

This article seeks to maintain a balance between depth and readability. It provides a systematic explanation of the essential concepts and methods of ODEs while covering their typical applications in language and vision tasks. Overall, this work can serve as an introductory guide to ODEs and their applications in deep learning.


## Resources

The full version of the article is available in pdf format: [[pdf]](./chapters/odes-in-vision-and-language.pdf).

We also provide individual chapters to facilitate reading:

<ul>
  <li>Chapter 1: Mathematical Preliminaries <a href="./chapters/chapter1-preliminaries.pdf" target="_blank">[pdf]</a></li>
  <li>Chapter 2: The ODE Perspective on Transformers <a href="./chapters/chapter2-ode-transformer.pdf" target="_blank">[pdf]</a></li>
  <li>Chapter 3: Neural ODEs and Flows <a href="./chapters/chapter3-neural-ode.pdf" target="_blank">[pdf]</a></li>
  <li>Chapter 4: Diffusion Models in Vision <a href="./chapters/chapter4-diffusion-models-in-vision.pdf" target="_blank">[pdf]</a></li>
  <li>Chapter 5: Diffusion Models in Language <a href="./chapters/chapter5-diffusion-models-in-language.pdf" target="_blank">[pdf]</a></li>
  <li>Chapter 6: Conclusions and Future Directions <a href="./chapters/chapter6-conclusions-and-future-directions.pdf" target="_blank">[pdf]</a></li>
</ul>

## Citation

To cite this article, please use the following BibTeX entry:

```bibtex
@article{xiao-etal:2026ode,
    title={Ordinary Differential Equations in Vision and Language},
    author={Tong Xiao, Junhao Ruan, Bei Li, Zhengtao Yu, Min Zhang and Jingbo Zhu},
    journal={???},
    year={2026}
}
```

## Contact

For any issues or comments, please feel free to contact the authors via e-mail: `xiaotong [at] mail.neu.edu.cn` or `rangehow [at] outlook.com`.
