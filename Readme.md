

# Prerequisites

- Quarto installed
- Git Installed
- GitHub Account created


## Timeline

08:00 - ca. 12:00

08:00 - 08:45: Introduction up to and including *3 Markdown*
08:50 - 09:35: *4 Quarto* and *5 Publishing HTML / Websites*
09:50 - 10:35: *6 Versioncontrol with Git / GitHub*
10:50 - 11:15: *6 Versioncontrol with Git / GitHub*
11:15 - 11:45: *Open Licensing*



## ffmpeg


within the folder "video"

    ffmpeg -ss 67.5 -i threema.mp4 -qscale:v 4 -frames:v 1 formatting.png -y
    ffmpeg -ss 69 -i threema.mp4 -qscale:v 4 -frames:v 1 formatted.png -y

    ffmpeg -i threema.mp4 -vcodec libx265 -crf 28 threema_low.mp4    # ← buggy             
    ffmpeg -i threema.mp4 -vcodec libx264 -crf 20 threema_low2.mp4   # ← better!             


# Topics

Reproducibility in Data Science

An irreproducible workflow:
- analyse unpublished the data in a proprietary GUI
- copy and paste your results into a text editor such as MS word
- share a pdf on dropbox


A reproducible workflow:
- analyse (self-) published the data with an open source scripting language (e.g. R)
- use literate programing to weave text and code (e.g. Quarto)
- share your code and results on a searchable website (e.g. GitHub)


- **R**: Helps us document the analysis process
- **Quarto**: Helps us explain the R code and interpret the results
- **Git**: Helps us version control our progress, do experiments and backup our code
- **GitHub**: Helps us collaborate with others, publish our code and our results

