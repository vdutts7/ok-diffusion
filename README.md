# ok-diffusion

Building a diffusion model from the ground up in hopes to better understand architecture. ControlNet's release a few weeks ago got my attention to how intricate and difficult it is to explain the blackbox of generative images a.k.a. AI art.

Documenting my path here. Been bad with that on other projects.

Let's see where this goes. 

Tools: Will be using pyTorch primarily.

## Context

ControlNet copies the weights of each block of Stable Diffusion into a trainable variant and a locked variant. The trainable variant can learn new conditions for image synthesis by fine-tuning with small data sets, while the blocked variant retains the capabilities of the production-ready diffusion model.

![image](https://user-images.githubusercontent.com/63992417/231795326-15eb4550-79b2-479e-bc26-8f19f49f420c.png)

_ControlNet models can, for example, derive edge lines from images and use them for further generation. | Image: Zhang, Agrawala_
