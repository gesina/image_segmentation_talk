# Talk on Image Segmentation with Mask R-CNN Network Architecture
These are the LaTeX sources of my lecture notes for a lecture in the seminar 
[*Topics in Machine Learning*](http://www.nullplug.org/ML-Blog/topics-in-machine-learning-seminar/) 
at the University of Regensburg in summer term 2018, supervised by
[Dr. Justin Noel](http://www.nullplug.org/)
which was held at 07/05/2018.
The precise topic is *Image Segmentation*.

If you have any questions on the topic or anything is unclear merely
from the material, please do not hesitate to open an issue.
The same applies of course in case you find any mistakes.

## Structure
As suggested in the official documentation of the 
[`beamer` LaTeX class for presentations](http://ftp.gwdg.de/pub/ctan/macros/latex/contrib/beamer/doc/beameruserguide.pdf)
the content can be found in a main file,
which is included by the purpose-specific compilation files.

- `image_segmentation.tex`: main content file
- `image_segmentation.bib`: bibliography
- `images/*`: image sources
- `image_segmentation-article.pdf`: latest compiled notes
- `image_segmentation-article.tex`: notes compilation file
- `image_segmentation-beamer.pdf`: latest compiled presentation
- `image_segmentation-beamer.tex`: presentation compilation file

## Compilation
(Tested) preliminaries: `TeXLive 2017` or `TeXLive 2018` distribution.

### Notes
For compilation of the notes execute the following commands
```bash
lualatex image_segmentation-article.tex
biber image_segmentation-article.tex
lualatex image_segmentation-article.tex
```

### Presentation
For compilation of the presentation slides execute

```bash
lualatex image_segmentation-beamer.tex
biber image_segmentation-article.tex
lualatex image_segmentation-beamer.tex
```
By default, this will be in 4:3 aspect ratio.
To change the aspect ratio, uncomment the corresponding options line
of the `\usepackage{beamer}` command within `image_segmentation-beamer.tex` 

## References
This talk was accompanied by an experimental implementation of Mask
R-CNN by me. 
See its [github repo](https://github.com/gesina/simple_mask_rcnn).

Any other references are listed in the bibliography file respectively
within the lecture notes .pdf file.
Image sources are referenced in the places they are included (look for
`\includegraphics`-commands respectively for the captions in the .pdf
file of the notes).

## License
As far as my research got, all used images were published under
non-restrictive License. Thus, I publish this under MIT License. 
