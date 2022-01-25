# Determining Bias to Search Engines from Robots.txt

The notebooks try to answer the following question:
  #### Does a robot bias exist?

Data was collected from CommonCrawl: 
  >an open repository of web crawl data that can be accessed and analyzed by anyone.

To answer the main question, the approach and algorithm suggested in the research paper [[1]](#1) were used.

The paper proposed > a quantitative metric to automatically measure robot biases.

Please refer to the paper for more details about the algorithm used to measure bias of one robots.txt file towards one search engine, in the notebook only an implementation of the algorithm is provided.

###### process_robotstxt.ipynb
This notebook is responsible for preprocessing of robots.txt files by:
- Loading them from disk
- Parse them
- Calculate their bias towards different crawlers
- Store the results in ".csv" format, to be analyzed later

###### robotstxt_analysis.ipynb
This notebook is reponsible for the analysis process and answering the following questions:
- What are the most favoured crawlers overall, and most disfavored crawlers.
- What is the most favored crawler in China (as Google is not the main cralwer, but Baidu is widely used)
- What is the most favored crawler in Russia (as Google is not the main crawler too, as Yandex is widely used)


## References
<a id="1">[1]</a> 
Sun, Y., Zhuang, Z., Councill, I. G., & Giles, C. L. (2007, November). Determining bias to search engines from robots. txt. In IEEE/WIC/ACM International Conference on Web Intelligence (WI'07) (pp. 149-155). IEEE.
