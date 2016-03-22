### This is where the content lives. Edit articles and content here.

#### You need:
1. the enlight-theme for Pelican
2. the output folder (see later)

Go to the content folder i.e. where this repository is and run Pelican:
``` pelican -o %OUTPUT_DIRECTORY% -t %WHERE_THEME_IS% ```

If you just have three folders called content, enlight-theme and output next to each other you can run
``` pelican -o ../output -t ../enlight-theme```

### Running a development server
As you write you will probably want to see how the website looks locally. From the output folder you can run a development server that serves its content locally. I have

```python -s SimpleHTTPServer 8080```

Then I can visit localhost:8080 from a browser to see how the site currently looks.

### Deployment
#### Making your changes go live
You need to be in the folder which is a git clone for *findenlight.github.io*. Github Pages understands to serve the page www.findenlight.github.io from whatever is the content of this repository.
So you need to be in a folder where you've put the repository findenlight.github.io, do `git commit -a` to commit all your changes and do ```git push```.
