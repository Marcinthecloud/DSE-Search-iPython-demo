# DSE Search iPython Notebook Demo

This is an iPython notebook demo that utilizes my Solr Amazon Book demo. 
There is examples of running DSE Search queries in Python. It's meant to work like a template to give you ideas on how to create your own applications with DSE, Python, and DSE Search. 


#####Prerequisites 
* Python 2.7+
* [iPython Notebook installed/configured](http://ipython.org/documentation.html)
* [DataStax Python Driver](https://github.com/datastax/python-driver) 
* [DataStax Enterprise 4.7.3 or greater](https://www.datastax.com/downloads) 
* [My Solr Amazon Book Demo installed/configured](https://github.com/Marcinthecloud/Solr-Amazon-Book-Demo)
* [Plot.ly installed and configured if you want to use the graphing functionality](https://plot.ly/)

#####How-to: 
1. Start DataStax Enterprise in search mode
  * ```for tarball installs: bin/dse cassandra -s```
  * ```for package installs: set SOLR=1 in the dse.default file and run: service dse start```
2. Run solr_dataloader.py from my Solr Amazon Demo
  * This will create the CQL schemas and load the data 
3. Run create_core.sh 
  * This will generate Solr cores and index the data
4. Open the Notebook in Jupyter and have fun! 

#####Why Plotly and not Matplotlib? 
Simply because I haven't implemented it yet. I'll put some templates for local graphs but for now, I enjoy the ease of use of Plotly as well as the functionality. 

