## Recent Advances in Machine Learning for Simulation Science

<h3>
    Aim
</h3>

<hr>

To organize research articles that pushes the boundary of **machine learning and (graph) neural networks for simulation** with the introduction of novel approaches, algorithms, or theoretical insights.

<hr>



## Building the Website

<pre>
> pip install -r requirements.txt
> make run
</pre>

When the code is ready to be deployed, run `make freeze` to get a static version of the website in the `build` folder. 

### Deploying to GitHub pages

- Define two command-line variables `GH_TOKEN` and `GH_REF`. `GH_TOKEN` is your Github personal access token, and will look like `username:token`. `GH_REF` is the location of this repo, e.g., ```$> export GH_REF=github.com/brownvc/neural-fields-review```.

- *DO NOT* add `GH_TOKEN` to the Makefile&mdash;this is your personal access token and should be kept private. Hence, declare a temporary command line variable using `export`.

- Commit any changes. Any uncommited changes will be OVERWRITTEN!

- Execute `make deploy`. 

- That's it.

  <hr>

### Repo Stub

The <a href="https://github.com/brownvc/neural-fields-review">repo</a> contains:

1) *Datastore* <a href="https://github.com/brownvc/neural-fields-review/tree/main/sitedata">`sitedata/`</a>

Collection of CSV files representing the papers, speakers, workshops, and other important information for the conference.

2) *Routing* <a href="https://github.com/brownvc/neural-fields-review/tree/main/main.py">`main.py`</a>

One file flask-server handles simple data preprocessing and site navigation. 

3) *Templates* <a href="https://github.com/brownvc/neural-fields-review/tree/main/templates">`templates/`</a>

Contains all the pages for the site. See `base.html` for the master page and `components.html` for core components.

4) *Frontend* <a href="https://github.com/brownvc/neural-fields-review/tree/main/static">`static/`</a>

Contains frontend components like the default css, images, and javascript libs.

5) *Scripts* <a href="https://github.com/brownvc/neural-fields-review/tree/main/scripts">`scripts/`</a>

<hr>

### Keyword Statistics
* Keyword Statistics: The keywords are generated by a JS script (paper_vis_statistics.js line 13-58) running on the front end every time this page is loaded. So yes they will change correspondingly when papers' data is updated.

<hr>