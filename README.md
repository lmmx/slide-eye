# slide-eye

Reproject lecture slides onto a screen in a low resolution lecture video
as a superresolution tactic

- Use [MiVOS](https://github.com/hkchengrex/MiVOS/) (CVPR 2021) to interactively
  define as many parts as needed to capture all speaker silhouette/shadow segments
  in the LR video
- Use SIFT (OpenCV/Kornia) for registration of known HR slide images
- Use Blender to reproject (as
  [in this example](https://matthewearl.github.io/2021/03/06/mars2020-reproject/))
