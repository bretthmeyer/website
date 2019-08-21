---
title: "Poster: Optimizing Keyword Spotting on Microcontrollers"
excerpt: "Undergraduate Adithya Lakshminarayanan presented his summer research at the SURE Poster Session today. It explores the different trade-offs inherent in quantizing models for keyword spotting. FP is best for top accuracy, but 8- and 16-bit models each strike interesting trade-offs under tighter constraints."
---

Undergraduate Adithya Lakshminarayanan presented his summer research at the McGill SURE Poster Session today.

## Abstract

Neural networks have become increasingly popular, due to their promise of state-of-the-art accuracy, in fields such as image and speech recognition. 
However, with the proliferation of resource-constrained edge computing platforms, in particular embedded devices and microcontrollers, it is also crucial to optimize for the memory utilization, compute, and latency. 
One method proposed to optimize neural networks is to quantize weights and biases i.e. reduce the precision of trainable parameters. 
We investigate the effects of using quantization on trade-offs between model accuracy and cost. 
In particular, we vary quantization format (8 bits, 16 bits, and 32 bits floating-point) and use design space exploration techniques to perform quantization-aware training using a speech dataset on CNN architectures. 
We note that the choice of quantization format is not a trivial one while attempting to optimize neuralnetworks with respect to several objectives; 
a single format does not prove dominant at all regions of the pareto-optimal front approximated from the results we obtain. 

Download the {% include icon-pdf.html link="/assets/pdfs/sure2019-alak.pdf" label="poster" %}.

Learn more about the {% include icon-www.html link="https://www.mcgill.ca/engineering/students/undergraduate/research" label="SURE Program" %} at McGill.

Follow {% include icon-twitter.html username="adithyalaks1" label="Adithya" %} on Twitter.
