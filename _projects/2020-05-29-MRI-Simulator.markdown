---
layout: single
title:  "MRI Simulator"
date:   2020-05-29 00:43:00 -0500
collection: projects
header:
    teaser: /assets/images/matrixImage.png
---

As my undergraduate thesis project I wanted to make a full simulation of the MRI process that was capable of running on both CPU and GPU. Maybe that sounds ambitious, but let us break the problem down. 

A real MRI scanner has an input, a program, and an output. Medically, that input is often a person's head. In reality, a lot of MRI research is done using samples called "phantoms". These are very simple samples that we know what they should look like as outputted images from our scanner. Phantoms let us test how well the scanner is working. The simplest phantom is a container of water. Since MRI works by exciting water molecules, and then detecting the signal emitted from them, we would expect to see the shape of the container on the output image. That is, if the scanner is working properly. If it isn't, we see a distorted image of that sample container.

If we can validate the output of MRI scanners using phantoms as an input, why do we want to simulate the process? Like a computer processing a job, an MRI scanner uses a program to run a scan. Writing successful programs for MRI scanners is a challenge, and a continued area of research. MRI scans can also be very time consuming, due to natural physical restrictions, which a simulation can fast forward through. A simulation can be used to verify and optimize these scanner programs, before they are ever used. A non-medical research MRI can cost $100s per hour to rent, so ensuring a valid program beforehand can also result in a significant cost savings to a lab.
