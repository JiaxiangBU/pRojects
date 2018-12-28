Project health
================
28 December, 2018 07:26:52

# Good practice

``` r
if(!require("goodpractice")){
  install.packages("goodpractice")
}
checks <- goodpractice::all_checks()
gp <- goodpractice::gp(fs::path_dir(getwd()),
                       checks[!grepl("rcmdcheck", checks)])
```

    ## 
    ##   
       checking for file ‘/tmp/Rtmp5G4e6o/remotes386a35e286a/pRojects/DESCRIPTION’ ...
      
    ✔  checking for file ‘/tmp/Rtmp5G4e6o/remotes386a35e286a/pRojects/DESCRIPTION’
    ## 
      
    ─  preparing ‘pRojects’:
    ## 
      
       checking DESCRIPTION meta-information ...
      
    ✔  checking DESCRIPTION meta-information
    ## 
      
       checking vignette meta-information ...
      
    ✔  checking vignette meta-information
    ## 
      
    ─  checking for LF line-endings in source and make files and shell scripts
    ## 
      
    ─  checking for empty or unneeded directories
    ## 
      
    ─  building ‘pRojects_0.0.1.9003.tar.gz’
    ## 
      
       
    ## 

``` r
print(gp)
```

    ## ── GP pRojects ────────────────────────────────────────────────────────────
    ## 
    ## It is good practice to
    ## 
    ##   ✖ write unit tests for all functions, and all package code in
    ##     general. 67% of code lines are covered by test cases.
    ## 
    ##     R/createPackageProject.R:55:NA
    ##     R/createPackageProject.R:56:NA
    ##     R/createPackageProject.R:57:NA
    ##     R/createPackageProject.R:93:NA
    ##     R/createPackageProject.R:136:NA
    ##     ... and 175 more lines
    ## 
    ## ───────────────────────────────────────────────────────────────────────────

# Typos

``` r
devtools::spell_check()
```

    ##   WORD              FOUND IN
    ## addin             README.md:40
    ##                   README.Rmd:36
    ## browseVignettes   pRojects.Rd:15
    ## codecov           createPackageProject.Rd:27
    ## config            createPackageProject.Rd:31
    ## flavours          BasicProjects.Rmd:12
    ## https             createAnalysisProject.Rd:37
    ##                   createBasicProject.Rd:35
    ##                   createPackageProject.Rd:40
    ##                   createTrainingProject.Rd:39
    ## md                BasicProjects.Rmd:28
    ## packrat           README.md:26,28
    ##                   README.Rmd:26,27
    ##                   TrainingProjects.Rmd:33
    ## Packrat           BasicProjects.Rmd:51
    ## PACKRAT           BasicProjects.Rmd:53
    ## param             createPackageProject.Rd:44
    ## pkgdown           createPackageProject.Rd:31
    ## pRoject           README.md:38
    ##                   README.Rmd:36
    ## README            createAnalysisProject.Rd:22,40
    ##                   createBasicProject.Rd:22,38
    ##                   createPackageProject.Rd:23,43
    ##                   createTrainingProject.Rd:20,42
    ##                   BasicProjects.Rmd:25,26,28
    ##                   RPackages.Rmd:23
    ## repo              createAnalysisProject.Rd:35,36
    ##                   createBasicProject.Rd:33,34
    ##                   createPackageProject.Rd:38,39
    ##                   createTrainingProject.Rd:37,38
    ## repostatus        createAnalysisProject.Rd:21
    ##                   createBasicProject.Rd:21
    ##                   createPackageProject.Rd:22
    ##                   createTrainingProject.Rd:19
    ## reproducibility   createAnalysisProject.Rd:24
    ##                   createBasicProject.Rd:24
    ##                   createTrainingProject.Rd:28
    ##                   README.md:26,28
    ##                   README.Rmd:26,27
    ## Reproducibility   BasicProjects.Rmd:48
    ## Rmd               BasicProjects.Rmd:25,28
    ## RStudio           README.md:36,38,40
    ##                   README.Rmd:35,36,36
    ##                   BasicProjects.Rmd:20,37
    ##                   TrainingProjects.Rmd:31
    ## travis            createAnalysisProject.Rd:38,39
    ##                   createBasicProject.Rd:36,37
    ##                   createPackageProject.Rd:41,42
    ##                   createTrainingProject.Rd:40,41
    ## usethis           createPackageProject.Rd:5,48
