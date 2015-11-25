# swirlify

swirlify is an R package that includes tools for writing and sharing swirl
courses. For more information on swirl, visit [our website](http://swirlstats.com) or our [GitHub repository](https://github.com/swirldev/swirl).

## Installation

```r
# If you don't have devtools installed run:
# install.packages("devtools")

library(devtools)
install_github(c("swirldev/swirl", "swirldev/swirlify"))
```

## Quick Start

We highly recommend using [RStudio](https://www.rstudio.com/) for authoring 
swirl content.

```r
library(swirlify)

# Create a new lesson and a new course
new_lesson("My Lesson", "My Course")

# Add content to the lesson in a text editor

# When you are finished writing your lesson, add it to the course manifest
add_to_manifest()

# Convret your course into a `.swc` file so you can share it easily.
pack_course()
```

## Documentation

For extensive documentation on swirlify and tips for writing swirl courses see
[the swirlify wiki](https://github.com/swirldev/swirlify/wiki).

## Course structure

swirl courses have the following structrue:

- **Courses** are directories that contain all of the files, folders, and lessons
associated with the course you are developing. The name of the course directory
is the name of the course. For example the name of the directory that
contains Team swril's R Programming course is named `R_Programming`.
- **Lessons** are directories that contain single units of instruction. The
name of a lesson directory is the name of that lesson. Every lesson must at
least contain a `lesson.yaml` file containing lesson content.
- **Questions** are written inside of the `lesson.yaml` file in each lesson
directory. Students are prompted with questions in sequential order.

## Contact

If you have any questions about using swirlify don't hesitate to reach out to us:
info@swirlstats.com