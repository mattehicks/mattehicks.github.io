## Metabolomics and Mass-Spectrometry applications

**Project description:** During my time working with Scripps Research Institute in La Jolla, CA; I was tasked with systems administration and software programming.  Allowing me to produce applications that would benefit the post-doctoral researchers, both locally and worldwide.  This was an interesting task, and a complex one.  
Users would be able to access the databases using custom "TSRI" Java libraries, and through web "REST" endpoints.   

### 1. Utilities and tools.

A series of java utilities were produced that would allow using strategies now commonly referred to as "Fuzzy-searches".  Where molecular compounds could be searched given a set of unkowns and envelope input.  This was done with Javascript, using hierarchical data result-sets, stored in JSON objects in cache memory.
Browser memory was very much in-demand, and thus the concept of big-data applications was introduced.

<img src="images/science1.png?raw=true"/>
<br>

### 3. Applications for mass-spectrometry, and "Metabolomics".

A dashboard was created for users to save their mass-spec result sets, and create reports and summaries based on findings.  This integrated well with the metabolite database that was growing quickly.  We were able to incorporate a 'categorical' mapping of metabolites, and corresponding user documents stored on this system.  Allowing for rough sketches in medical and bioscience thesis and investigations, coined as "Untargeted Metabolomics" research.

<img src="images/science3.png?raw=true"/>
<br>

### 3. Security

A number of php and python was written to strengthen the backend servers, and place restrictions on download and data limits.
This had to be solved in a creative manner, as most normal users were downloading very large datasets, and sessions lasting for hours at a time, while other nefarious bad-actors were actively trying to steal data and cause malicious activity within the data-service layer.  Snort software was eventually deployed on the network, which could effectively profile users normal activity, and could dynamically identify users that were violating agreements, and take appropriate action.

<img src="images/science2.png?raw=true"/>