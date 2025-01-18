# EpiFusion Framework Software Vignettes

This repository holds the code and data used for a series of vignettes on using the EpiFusion Analysis Framework to analyse some simulated outbreak datasets. By cloning this repository, extra manuscript assets (e.g. diagrams created outside R) are also made available to compile the manuscript ([`full_manuscript.Rmd`](https://github.com/ciarajudge/EpiFusion_Vignettes/blob/main/full_manuscript.Rmd)) and supplementary information ([`supplementary_info.Rmd`](https://github.com/ciarajudge/EpiFusion_Vignettes/blob/main/supplementary_info.Rmd)). Alternatively, each vignette is provided separately in Rmd files, should you wish to work through each individually.

## Installing Java
If you don't have Java installed on your machine, you will need to do this in order to follow the tutorials in this repository. Simply go to the [Java website](https://www.java.com/en/download/help/download_options.html) and download the appropriate release for your machine. To check the software has installed correctly, open a console window and type the command `java`. You should see something that looks like this.

```
Usage: java [options] <mainclass> [args...]
           (to execute a class)
   or  java [options] -jar <jarfile> [args...]
           (to execute a jar file)
   or  java [options] -m <module>[/<mainclass>] [args...]
       java [options] --module <module>[/<mainclass>] [args...]
           (to execute the main class in a module)
   or  java [options] <sourcefile> [args]
           (to execute a source-file program)

 Arguments following the main class, source file, -jar <jarfile>,
 -m or --module <module>/<mainclass> are passed as the arguments to
 main class.
```
Making sure that 

## Installing EpiFusionUtilities
To install EpiFusionUtilities you can use the `install_github` command. In R, that looks like this:

  ```
  devtools::install_github("https://github.com/ciarajudge/EpiFusionUtilities")
  ```

We recommend also consulting the [full function reference on the package website](https://ciarajudge.github.io/EpiFusionUtilities/reference/index.html) where there is lots of useful instructions on how to use `EpiFusionUtilities` to interact with the EpiFusion software.

## Vignette 1: Full Workflow
In the first vignette we demonstrate a full workflow that uses EpiFusion and EpiFusionUtilities to analyse a simple simulated dataset. This includes detailed examples of the steps of the process:

* Data Loading
* Data Preparation
* Running EpiFusion
* Loading Results
* Plotting Results
* Inspecting Parameter Posteriors and Convergence Statistics

You can work through this vignette using the [`full_workflow.Rmd`](https://github.com/ciarajudge/EpiFusion_Vignettes/blob/main/full_workflow.Rmd) script.

## Vignette 2: Examining Phylogenetic Uncertainty
In the second vignette we show how to utilise a tree posterior as the data input into EpiFusion to allow exploration of the effect of phylogenetic uncertainty on the results. This vignette is in the [`phylogenetic_uncertainty.Rmd`](https://github.com/ciarajudge/EpiFusion_Vignettes/blob/main/phylogenetic_uncertainty.Rmd) script.

## Vignette 3: Time-variant Prior Parameterisation
In the final vignette we explain how to introduce more advanced parameterisation by setting time-variant priors to parameterise a step-change in the sampling rate over time. You can work through this vignette using the [`sampling_step_change.Rmd`](https://github.com/ciarajudge/EpiFusion_Vignettes/blob/main/full_manuscript.Rmd) script.









