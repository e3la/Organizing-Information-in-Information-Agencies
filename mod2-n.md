---
jupyter:
  jupytext:
    text_representation:
      extension: .md
      format_name: markdown
      format_version: '1.3'
      jupytext_version: 1.10.2
  kernelspec:
    display_name: Python 3
    language: python
    name: python3
---

# Key Ideas in IR: Measuring Success: Precision and Recall

Imagine you've been using the ERIC database ([https://eric.ed.gov/](https://eric.ed.gov/)) to search for content in the collection. You first used the the thesaurus of descriptors ([https://eric.ed.gov/?ti=all](https://eric.ed.gov/?ti=all)) and found descriptors that fit what you need. You carried out your search, and the three of the results seem perfect.

You wonder, however—are there more results that were overlooked? The video you watched about searching in ERIC mentioned that sometimes items can be relevant, but are not retrieved.

As in the video, you change the limiters of the query, and retrieve three additional articles. Though they are not by the author you wanted, they seem relevant. You now have a total of six articles.

The first query is an example of high precision, but low recall. All three of the original results were really good, but out of all the articles indexed in the database, some other good results were not retrieved.

\*\*\*

Later, you carry out the same search in [Google Scholar](https://scholar.google.com/). You end up with 10 results on the first page, but only two articles are by the author you intended and on the topic you are studying. In this instance, your initial results set had low precision. It might also have had low recall.

## Measuring Success in Retrieval

What do **precision** and **recall** mean? In a database environment, like ERIC, or the databases a library subscribes to, or the library catalog (rather than the entire web), there are a certain number of relevant documents and are often numerous ways for users to query the database. 

#### Measures of Precision

Your results set has high precision if the results all are about what you intend. If you search for Java and want information about the Island nation, do the eight results meet your need?  Imagine that they do. In this case, the search had high precision.

Below is the definition of [precision](https://products.abc-clio.com/ODLIS/odlis_p.aspx#precision) from the ODLIS: 

> **precision**  
> In [information retrieval](https://products.abc-clio.com/ODLIS/odlis_i.aspx#inforetrieval), a measure of [search](https://products.abc-clio.com/ODLIS/odlis_s.aspx#search) effectiveness, expressed as the ratio of [relevant](https://products.abc-clio.com/ODLIS/odlis_r.aspx#relevance) [records](https://products.abc-clio.com/ODLIS/odlis_r.aspx#record) or [documents](https://products.abc-clio.com/ODLIS/odlis_d.aspx#document) retrieved from a [database](https://products.abc-clio.com/ODLIS/odlis_d.aspx#database) to the total [number](https://products.abc-clio.com/ODLIS/odlis_n.aspx#number) retrieved in response to the [query](https://products.abc-clio.com/ODLIS/odlis_q.aspx#query); for example, in a database containing 100 records relevant to the [topic](https://products.abc-clio.com/ODLIS/odlis_t.aspx#topic) "book history," a search retrieving 50 records, 25 of which are relevant to the topic, would have 50 percent precision (25/50). Synonymous with _relevance ratio_. Compare with [recall](https://products.abc-clio.com/ODLIS/odlis_r.aspx#recall). **_See also_**: [fallout](https://products.abc-clio.com/ODLIS/odlis_f.aspx#fallout).

Now, imagine the opposite scenario—that results you got did not meet your needs. You were looking for information about coffee, and all results pertained to the island. In that case, the search would have yielded results that were not relevant. These are called "false drops."

The ODLIS defines [false drops](https://products.abc-clio.com/ODLIS/odlis_f.aspx#falsedrop) in the following way:

> **false drop**  
> In [information retrieval](https://products.abc-clio.com/ODLIS/odlis_i.aspx#inforetrieval), a [bibliographic record](https://products.abc-clio.com/ODLIS/odlis_b.aspx#bibrecord) retrieved in a [keywords](https://products.abc-clio.com/ODLIS/odlis_jk.aspx#keywords) [search](https://products.abc-clio.com/ODLIS/odlis_s.aspx#search) that is unrelated to the [subject](https://products.abc-clio.com/ODLIS/odlis_s.aspx#subject) of the search, usually because it meets the [syntactic](https://products.abc-clio.com/ODLIS/odlis_s.aspx#syntax) requirements of the [query](https://products.abc-clio.com/ODLIS/odlis_q.aspx#query) but not its [semantic](https://products.abc-clio.com/ODLIS/odlis_s.aspx#semantics) requirements. False drops generally occur when meaning is contingent on the order of [search terms](https://products.abc-clio.com/ODLIS/odlis_s.aspx#searchterm) (library + school retrieves "library school" and "school library") or when a [term](https://products.abc-clio.com/ODLIS/odlis_t.aspx#term) used in a [search statement](https://products.abc-clio.com/ODLIS/odlis_s.aspx#searchstatement) has more than one meaning. For example, a search on the keyword "aids" will retrieve records for [items](https://products.abc-clio.com/ODLIS/odlis_b.aspx#bibitem) about HIV infection and also items about _hearing aids_, _teaching aids_, _band-aids_, etc. To avoid this problem, a [qualifier](https://products.abc-clio.com/ODLIS/odlis_p.aspx#parenthetical) such as "disease" must be added to the [search statement](https://products.abc-clio.com/ODLIS/odlis_s.aspx#searchstatement) to make retrieval more [precise](https://products.abc-clio.com/ODLIS/odlis_p.aspx#precision). Synonymous with _false combination_. **_See also_**: [semantic factoring](https://products.abc-clio.com/ODLIS/odlis_s.aspx#semanticfactoring).

Measures of precision, therefore, can be subjective. What is relevant to one person might not be relevant to another. The question of relevance can be difficult to define, because it is subjective, too.

#### Measures of Recall

Out of the entire database of articles, how many of the articles about the island nation did you retrieve? Imagine that in reality there are 60 articles on Java the country, but you only retrieved eight. In that case, your search results were not very thorough and you had very low recall.

The relevant definition of [recall](https://products.abc-clio.com/ODLIS/odlis_r.aspx#recall) in the ODLIS is the following:

> In [information retrieval](https://products.abc-clio.com/ODLIS/odlis_i.aspx#inforetrieval), a measure of the effectiveness of a [search](https://products.abc-clio.com/ODLIS/odlis_s.aspx#search), expressed as the ratio of the [number](https://products.abc-clio.com/ODLIS/odlis_n.aspx#number) of [relevant](https://products.abc-clio.com/ODLIS/odlis_r.aspx#relevance) [records](https://products.abc-clio.com/ODLIS/odlis_b.aspx#bibrecord) or [documents](https://products.abc-clio.com/ODLIS/odlis_d.aspx#document) retrieved in response to the [query](https://products.abc-clio.com/ODLIS/odlis_q.aspx#query) to the total number of relevant records or documents in the [database](https://products.abc-clio.com/ODLIS/odlis_d.aspx#database); for example, in a database containing 100 records relevant to the [topic](https://products.abc-clio.com/ODLIS/odlis_t.aspx#topic) "book history," a search retrieving 50 records, 25 of which are relevant to the topic, would have 25 percent recall (25/100). One of the main difficulties in using recall as a measure of search effectiveness is that it can be nearly impossible to determine the total number of relevant records in all but very small databases. Compare with [precision](https://products.abc-clio.com/ODLIS/odlis_p.aspx#precision). **_See also_**: [fallout](https://products.abc-clio.com/ODLIS/odlis_f.aspx#fallout).

The way that information is organized and searched can have an effect on how high or low the precision of the results is, and how high or low the recall is. As a result, information professionals strive to organize materials to promote precision (see Part II of this class for more information) and they learn how information is stored in a database so that they are more adept at formulating queries that promote high recall.

#### **Next**

_Next, a blog post will reinforce your understanding of these concepts by applying them in a slightly different environment._

```python

```
