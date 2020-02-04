
# add PUC repo
#r <- getOption("repos")
#r["CRAN"] <- "http://dirichlet.mat.puc.cl"
#options(repos=r)
#rm(r)

# set cairo display
setHook(packageEvent("grDevices", "onLoad"),
        function(...) grDevices::X11.options(width=8, height=8, 
                                             xpos=0, pointsize=10, 
                                             type="nbcairo"))  # Cairo device
                                             #type="cairo"))    # other Cairo dev
                                             #type="xlib"))      # old default

# change prompt
options(prompt="R> ", digits=4, show.signif.stars=FALSE)

# change pdf viewer
options("pdfviewer"="xpdf")

# this gets run on startup 
.First <- function() {
    cat ("TINY LEMONS\n")
}

# this gets run when finishing
#.Last <- function() {
#    if (!any(commandArgs()=='--no-readline') && interactive()) {
#        require(utils)
#        try(savehistory(Sys.getenv("R_HISTFILE"))
#    }
#}

# Override q() to not save by default. Same as saying q("no").
#q <- function (save="no", ...) {
#    quit(save=save, ...)
#}

# avoid save question
#require(Defaults)
#setDefaults(q, save="no")
#useDefaults(q)

# Sys.getenv doesn't seem to work with fish...
#tryCatch(
#  {options(
#      width = as.integer(Sys.getenv("COLUMNS")))},
#  error = function(err) {
#    write("Can't get your terminal width. Put ``export COLUMNS'' in your \
#           .bashrc. Or something. Setting width to 120 chars",
#           stderr());
#    options(width=120)}
#)

# Column width. Find out how to use tput cols for this
options(width=266)

# some aliases
cd <- setwd
pwd <- getwd


