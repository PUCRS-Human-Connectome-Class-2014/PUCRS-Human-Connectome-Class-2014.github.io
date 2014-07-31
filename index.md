---
layout: page
title: Homepage
---

#Overview

This is the homepage for the course **Mapping the Connectivity of the Human Brain** which will occur July 28 - 31 at the Pontifícia Universidade Católica do Rio Grande do Sul, in Porto Alegre, Brazil. Lectures for the course are scheduled for 17:00 to 20:00 each evening and will be held in room `302 Bloco B` of the School of Engineering building (`building number 30`). Electrical engineering students at PUCRS who are enrolled in *0407-03: Instrumentação Biomédica e Imagens Médicas* will receive 1 credit hour for completing this course. This course will be taught exclusively in English.

##Instructors:
 - [Cameron Craddock, PhD](mailto:cameron.craddock@gmail.com) - Research Scientist VI, Nathan S. Kline Institute for Psychiatric Research and Director of Imaging, Child Mind Institute, New York, NY
 - [Alexandre Franco, PhD](mailto:alexandre.franco@pucrs.br) - Associate Professor at Pontifícia Universidade Católica do Rio Grande do Sul (PUCRS) and Coordinator of Research in Neuroinformatics and Image Post-processing at the Brain Institute of Rio Grande do Sul (InsCer)
 
##Teaching Assistants
- [Caroline Froehlich](mailto:CAROL.FROHLICH@GMAIL.COM), Graduate program in Computer Science, PUCRS
- [Nathassia Aurich](mailto:nathassia.aurich@acad.pucrs.br), Graduate program in Electrical Engineering, PUCRS
- [Guilherme Peixoto](mailto:guilherme.peixoto@acad.pucrs.br), Undergraduate program in Physics, PUCRS

#Background

Mapping the human connectome is an important next step in neuroscience that promises to transform our understanding of the brain (Craddock et al. 2013). The connectome is a complete map of neural connections in the brain and consists of distinct brain regions, their anatomical connections, and the functional interactions. Among the techniques that can be used for measuring the connectome, magnetic resonance imaging (MRI) is dominant, due to its widespread availability, safety, and spatial resolution. Anatomical connections between brain regions are commonly inferred from diffusion-weighted MRI (dMRI) and their functional interactions are inferred from functional MRI (fMRI). Once the data is collected a variety of analysis methods can be employed extract connectivity information (Varoquaux and Craddock, 2013) and to link variability in these connections to intra-individual variation in phenotypic variables (Kelly et al. 2011; Castellanos et al. 2013).

This course will provide an in-depth review of the neuroimaging and analytical methods for mapping the human connectome. It will begin with an overview of the physics behind MRI, dMRI, and fMRI, and the preprocessing techniques that are required to make the data comparable across observations. It will then cover the mathematical techniques for inferring functional and structural connectivity from the data, and for comparing this data across individuals. This will be performed in a mathematical framework that treats the connectome as a graph, in which nodes represent brain regions, and edges between nodes represent functional and structural connections. Advanced topics will be covered such as pattern based classification approaches, as well as multi-modal techniques that integrate information from function and structure. Each lecture will end with laboratory exercises aimed translating the covered information into practical skills.

#Syllabus


##Monday, July 28, 17:00 to 20:00
- **Lecture**: 
    - Basics of MRI physics, functional MRI, and diffusion MRI. [slides](http://pucrs-human-connectome-class-2014.github.io/MRI_lecture_slides/index.html)
- **Lab**: 
    - [Lab #1: Working with neuroimaging data using Python and Nipy](labs.html#lab1) 
    - [Lab #2: Open Science resources for connectomes research](labs.html#lab2)
- **Reading**:
    - [Craddock, R. C., Jbabdi, S., Yan, C., Vogelstein, J. T., Castellanos, F. X., Di Martino, A., Kelly, C., Heberlein, K., Colcombe, S., & Milham, M. P. (2013). **Imaging human connectomes at the macroscale**. *Nature Methods*, 10(6), 524–539.](papers/ImagingHumanConnectomesAtTheMacroscale.pdf) - A good overview of connectomics from image acquisition through analysis and provides some prospectives on what can be learned from connectomics.
    - [Buxton, R. B. (2012). **Dynamic models of BOLD contrast**. *NeuroImage*, 62(2), 953–61.] (https://www.physast.uga.edu/files/phys4510_zhao/No6%20dynamic%20models%20of%20BOLD%20contrast.PDF) - Describes various physiological models of how neuronal activity results in the signal we measure with fMRI.
    - [Beaulieu, C. (2002). **The basis of anisotropic water diffusion in the nervous system - a technical review**. *NMR Biomed*, 15(7-8), 435–455.](papers/BasisOfDiffusion.pdf) - Detailed information on the relationship between diffusion MRI and neuroanatomy  
    
##Tuesday, July 29, 17:00 to 20:00
- **Lecture**: 
    - Building connectomes from fMRI data - preprocessing and functional connectivity [slides](http://pucrs-human-connectome-class-2014.github.io/fMRI_connectome_slides/index.html)
- **Lab**:
    - [Lab #3: Preprocessing fMRI data using CPAC](labs.html#lab3)
    - [Lab #4: Mapping functional connectome from fMRI](labs.html#lab4)
- **Reading**:
    - [Biswal, B., Yetkin, F. Z., Haughton, V. M., & Hyde, J. S. (1995). **Functional connectivity in the motor cortex of resting human brain using echo-planar MRI**. *Magnetic Resonance in Medicine*, 34(4), 537–41.](papers/FunctionalConnectivityMotorCortexRestingBrain.pdf) - The first report of resting state functional connectivity
    - [Strother, S. C. (2006). **Evaluating fMRI Preprocessing Pipelines**. *IEEE Engineering in Medicine and Biology Magazine*, 25(2), 27–41.](papers/EvaluatingFMRIPreprocessingPipelines.pdf) - Describes fMRI preprocessing methods and their optimization
    - [Margulies, D. S., Böttger, J., Long, X., Lv, Y., Kelly, C., Schäfer, A., … Villringer, A. (2010). **Resting developments: a review of fMRI post-processing methodologies for spontaneous brain activity**. *MAGMA*, 23(5-6), 289–307.](papers/RestingDevelopments.pdf) - A nearly comprehensive review of functional connectivity analyses 
    - [Kelly, C., Biswal, B. B., Craddock, R. C., Castellanos, F. X., & Milham, M. P. (2012). **Characterizing variation in the functional connectome: promise and pitfalls**. *Trends in Cognitive Sciences*, 16(3), 181–8.](papers/CharacterizingVariationInTheFunctionalConnectomePromiseAndPitfalls.pdf) - Describes the application of functional connectivity for understanding inter-individual variations in brain function and many of the open issues plaguing funcitonal connectivity analyses
    
##Wednesday, July 30, 17:00 to 20:00
- **Lecture**: 
    - Building connectomes from dMRI data - preprocessing and tractography [slides](http://pucrs-human-connectome-class-2014.github.io/DTI_connectome_slides/index.html)
- **Lab**:
    - [Lab #5: Mapping structural connectomes from dMRI](labs.html#lab5)
- **Reading**:
    - [Soares, J. M., Marques, P., Alves, V., & Sousa, N. (2013). **A hitchhiker’s guide to diffusion tensor imaging**. *Frontiers in Neuroscience*, 7, 31.](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3594764/) - A detailed review of diffusion imaging and its analysis
    - [Zalesky, A., Fornito, A., Harding, I. H., Cocchi, L., Yücel, M., Pantelis, C., & Bullmore, E. T. (2010). **Whole-brain anatomical networks: does the choice of nodes matter?** *NeuroImage*, 50(3), 970–83.](papers/WholeBrainAnatomicalNetworks.pdf) - Describes creating graphs from DTI data and the impact of node selection on these graphs
    - [Jones, D. K., Knösche, T. R., & Turner, R. (2013). White matter integrity, fiber count, and other fallacies: the do’s and don'ts of diffusion MRI. NeuroImage, 73, 239–54.](http://ac.els-cdn.com/S1053811912007306/1-s2.0-S1053811912007306-main.pdf?_tid=1c73a1c4-1474-11e4-a4ab-00000aab0f01&acdnat=1406345145_23539d0f533cca7b7ae59d775c064bd3) - Another review of diffusion MRI that focuses on common misinterpretations of the data

##Thrusday, July 31, 17:00 to 20:00
- **Lecture**: 
    - Comparing connectomes - graph theory, statistical learning, classifiers, and correcting for multiple comparisons
- **Lab**: 
    - [Lab #6: Calculating graph statistics](labs.html#lab6)
- **Reading**:
    - [Rubinov, M., & Sporns, O. (2010). **Complex network measures of brain connectivity: uses and interpretations**. *NeuroImage*, 52(3), 1059–69.](http://brainimaging.waisman.wisc.edu/~chung/neuro.processing/literature/rubinov.2010.NI.network.pdf) - Defines many of the different graph measures that are used in connectomics.
    - [Richiardi, J., Achard, S., Bunke, H., & Van De Ville, D. (2013). **Machine Learning with Brain Graphs: Predictive Modeling Approaches for Functional Imaging in Systems Neuroscience**. *IEEE Signal Processing Magazine*, 30(3), 58–70.](http://miplab.epfl.ch/pub/richiardi1301.pdf) - Discusses the application of machine learning algorithms to the connectome.
    - [Shehzad, Z., Kelly, C., Reiss, P. T., Craddock, R. C., Emerson, J. W., McMahon, K., … Milham, M. P. (2014). **A multivariate distance-based analytic framework for connectome-wide association studies**. *NeuroImage*, 93 Pt 1, 74–94.](http://ac.els-cdn.com/S1053811914001232/1-s2.0-S1053811914001232-main.pdf?_tid=8cacba38-159c-11e4-b1ce-00000aab0f27&acdnat=1406472464_c2dc1062163b925178790341ba463b17) - Multivariate technique for finding associations between interindividual variability and features of the connectome.

#Grading
Grades for students who are enrolled in *0407-03: Instrumentação Biomédica e Imagens Médicas* will be determined based on class attendance and a class [project](project.html).
