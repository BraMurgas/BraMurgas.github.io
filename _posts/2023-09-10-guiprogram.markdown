---
layout: post
title:  "How am I creating a GUI for a microstructure generator?"
date:   2023-09-10 16:33:00 +0100
categories: MyWork
---

I've been working for a while with microstructure generation. It's the first step before running simulations. I've worked with Dream3D, some in-house codes and Neper. They all have their own advantages and disadvantages.

Let's start with that. Dream3D has a friendly interface but the pipelines are really rigid.

| Program         | Advantage     | Disadvantage |
|--------------|-----------|------------|
| Dream3D | Nice GUI and user friendly      | The data structure is rigid        |
| Neper      | Python and nice plots  | Limited view of the microstructure       |
| In-house      | C++/Fortran and flexible  | Not open source       |

I like Dream3D a lot, it's really mature but I think it needs some improvements. For the Cold-Spray project I needed to couple a Generative Adversarial Network with the grain packer. It took me and my coworker a monumental amount of work to made it work. I know there is a python binder for Dream3D, but I was unable to use it properly. 

So here is the list of requirements for this project:

* First of all, it needs to be open source 
* It need a GUI to see the microstructures. Also, I want to use Paraview to visualize the files. 
* It need a python binder in order to couple it easy with machine learning models. I recently saw a way to run ML models with c++ but the binder is important.

The first question that came into my mind. How to create the GUI? I starting my research on internet and saw a bunch of projects with a GUI. I've been impressed with the work of Bruno Levy, from the INRA in Nancy, France. He has develop a wonderful tool called Geogram and the GUI was developed using ImGui. 

Under construction...

Author: Brayan David Murgas Portilla. This text are notes on the progress of a project I started a while ago.
