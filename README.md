# slide-eye

Reproject lecture slides onto a screen in a low resolution lecture video
as a superresolution tactic

- Use [MiVOS](https://github.com/hkchengrex/MiVOS/) (CVPR 2021) to interactively
  define as many parts as needed to capture all speaker silhouette/shadow segments
  in the LR video
- Use SIFT (OpenCV/Kornia) for registration of known HR slide images
  - See [slides](https://drive.google.com/file/d/1o1YwDI61SJYCoEn2t5DwH3C7pP6KvBNF/view)
    and [video](https://drive.google.com/file/d/10qGr4Eek6W3w7trElCg45brC2JCtFLqW/view)
    from Dmytro Mishkin (March 2021)
    - In fact this is a higher resolution example to consider, with a mouse cursor
      instead of a silhouette
- Use Blender to reproject (as
  [in this example](https://matthewearl.github.io/2021/03/06/mars2020-reproject/))

## Other ideas

- Instead of reprojecting video, possible to play the video under a masked image somehow?
  - Since the slides are unchanging, do not create a video sequence (expensive), instead
    overlay them where unobscured using a mask (e.g. SVG surely has such a feature?)
  - Do not want to end up converting PDF to HTML
  - For higher quality videos it'll be preferable to upsample to HD video rather than
    have an experimental SVG overlay interface (simpler to upload to YouTube than manage)
    although if this worked well it would no longer require YouTube and permit self-host
