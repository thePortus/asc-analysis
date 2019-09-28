# Anglo-Saxon Charters Database Analysis

*DH Scraping and Analyzing the ASC database with Jupyter Notebooks*

[David J. Thomas](mailto:dave.a.base@gmail.com), [thePortus.com](http://thePortus.com)<br />
Instructor of Ancient History and Digital Humanities,<br />
Department of History,<br />
[University of South Florida](https://github.com/usf-portal)

---

**Run this demonstration in-browser with Binder**

<a alt="Binder" href="https://mybinder.org/v2/gh/thePortus/asc-analysis/master" target="_blank"><img src="https://mybinder.org/badge.svg" /><a/>

You don't even need to clone this repo manually. Click the Binder icon above and Binder will clone the repo and let you run it in browser. Run the scripts, generate the exportable data, and download the results to your local computer!

---

Together, the [Anglo-Saxon Charter (ASC)](http://aschart.kcl.ac.uk) and the [Prosopography of Anglo-Saxon England (PASE)](http://pase.ac.uk/) databases contain massive amounts of information on individuals and sources of individuals in England from 600-900 AD. These workbooks will show you how to use Python3 to scrape these two databases and explore and analyze the data in new ways using network and text analysis. This exercise will focus on charters, legal documents which framed power, and the people in them. We will use the `requests` and `BeautifulSoup` modules to fetch and parse information, `networkx` to perform network analysis, and finally the `nltk` and `cltk` modules to do some text analysis on the documents themselves.

![Banner image](../assets/network-banner.png)

*A network of nearly 2,500 Anglo-Saxons, connected by appearing together as witnesses in over 600 medieval documents.*

---

Medieval charters were documents of importance and power. They bound institutions and powerful individuals together and created links that were displayed to wider communities. These charters were usually grants of land, often from a king, to a monastery, individual, or some other institution. These charters were critical documents in the distribution of land and goods, and all contained witnesses whose authority guarunteed the legitimacy of these documents. You can clearly see the lists of witnesses outlined in the image below.

---

![Image of manuscript outlining witnesses](../assets/charter-large.jpg)

While appearing together hardly means that there is any real connection between two witnesses, it does mean that they were openly connected and that their social authority was indirectly bound toegether. The goal of these workbooks is to unravel the connections and individuals bound up in these charters. The goal is also to show you what can be done with an existing data source if you explore it in a new way.

---

Installation...

```sh
# clone the repo and move inside the directory
git clone https://github.com/thePortus/asc-analysis && cd asc-analysis

# install python requirements
pip install -r requirements.txt

# launch notebook
jupyter notebook
```

If a new tab did not already open in your browers, navigate to
http://localhost:8000

Finally, open `notebooks/1-scrape.ipynb` to get started
