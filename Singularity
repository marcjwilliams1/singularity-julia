Bootstrap: docker
From: jupyter/datascience-notebook

%labels
  Maintainer Marc J Williams

%help
  Singularity image for following paper:

%post
  # add R packages from CRAN
  Rscript -e "install.packages(pkgs = c('ggplot', 'cowplot', 'readr'))"

  # add R packages from github
  Rscript -e "library(devtools); install_github('marcjwilliams1/dndscv', ref = 'dev')"

  #add julia packages
  julia -e "import Pkg; Pkg.add(\"Distributions\")"
