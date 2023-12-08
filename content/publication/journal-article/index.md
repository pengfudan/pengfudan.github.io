---
title: "Oriented Object Detection Based on Foreground Feature Enhancement in Remote Sensing Images"
authors:
- Peng Lin
- Xiaofeng Wu
- Bin Wang
# author_notes:
# - "Equal contribution"
# - "Equal contribution"
date: "2022-11-05T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2022-12-08T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "*Journal of Source Themes, 1*(1)"
publication_short: ""

abstract: Oriented object detection is a fundamental and challenging task in remote sensing image analysis and has received much attention in recent years. Optical remote sensing images often have more complex background information than natural images, and the number of annotated samples varies in different categories. To enhance the difference between foreground and background, current one-stage object detection algorithms attempt to exploit focus loss to balance the foreground and background weights, thus making the network more focused on the foreground part. However, the current one-stage object detectors still face two main challenges:(1) the detection network pays little attention to the foreground and does not make full use of the foreground information; (2) the distinction of similar object categories has not attracted attention. To address the above challenges, this paper presents a foreground feature enhancement method applied to one-stage object detection. The proposed method mainly includes two important components:keypoint attention module (KAM) and prototype contrastive learning module (PCLM). The KAM is used to enhance the features of the foreground part of the image and reduce the features of the background part of the image, and the PCLM is utilized to enhance the discrimination of samples between foreground categories and reduce the confusion of samples between different categories. Furthermore, the proposed method designs and adopts an equalized modulation focal loss (EMFL) to optimize the training process of the model and increase the loss weight of the foreground later in the model training. Experimental results on the publicly available DOTA datasets and HRSC2016 datasets show that our method exhibits state-of-the-art performance.


# Summary. An optional shortened abstract.
summary: This paper has presented the foreground feature enhancement method for one-stage anchor-free oriented object detector, which is more robust and easier to migrate to other models than the anchor-based method. The O2DFFE method mainly consists of three parts. The first part is the designed KAM. It can be used to enhance the features of the foreground portion of the image and weaken the features of the background portion of the image. The second part is the designed PCLM, applied on the classification branch, makes the different classes of foreground features as orthogonal as possible in the feature space. It can be utilized to enhance the discrimination of samples between different categories, thereby reducing the confusion of samples between different categories. The third part is the constructed EMFL. It can be adopted to improve the learning process of the model for positive and negative samples. The results on the DOTA and HRSC2016 datasets show that the proposed method outperforms existing methods, and can achieve the accurate detection results of the two-stage target detection method with a fast calculation speed. In future work, we may try to replace the backbone of the proposed method with the form of Transformer [42] to achieve a new object detection framework that makes the model more fully utilized for the foreground information, so that we can obtain the features of the global spatial attention.

tags:
- Source Themes
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: https://www.mdpi.com/2072-4292/14/24/6226
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/jdD8gXaTZsc)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---

{{% callout note %}}
Click the *Cite* button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/).
