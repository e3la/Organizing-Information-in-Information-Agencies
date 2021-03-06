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

<!-- #region id="zChsJoUwu9VR" -->
# Key Ideas in IR: Controlled Vocabularies and Thesauri

## Controlled Vocabularies

Certain fields in databases may contain information that must be formatted in a certain way. Contacts in a phone include information about a person, such as name, phone number, etc. Some Contacts might only allow calendar dates to be entered in the Birthday field of a record for a friend, or digits to appear in the phone number field.

Information agencies do something similar when they provide searchable content in a field from a controlled vocabulary such as the Library of Congress Subject Headings (LCSH) or the name authorities. Only terms from the controlled vocabulary may be included. In the example above, there are 12 months from which to choose for date information. In information agencies, controlled vocabularies provide similar lists of allowed information. Usually, instead of months, controlled vocabularies are lists of topics a book might be about, or names of authors (often with the last name first), or genres (e.g., Westerns, etc.). These controlled vocabularies are created by organizations and are added to records by information professionals. 

Controlled vocabularies are made up of established preferred terms that a cataloger or indexer select when assigning descriptors to a record. They indicate the content of the work. Often synonyms are included as lead-in vocabulary - conceptualized simply as SEE ALSO. Works being cross-referenced is of great help to users. Imagine a book about light bulbs titled _The Bright Incandescent Globe_, if it is cross-referenced with Light Bulb, than a search for light bulb should be directed also to this oddly titled book. 

Vocabulary control is the process of creating and maintaing a list of preferred terms. They are often listed alphabetically in subject headings list, or indexing terms in a thesaurus. A study by [Tina Gross and Arlene G. Taylor (College & Research Libraries, May 2005.)](https://doi.org/10.5860/crl.66.3.212) found that more than one-third of records retrieved successfully would be lost if subject headings had not been present.

As easy as it is to search Amazon and get good results, results may not yield desired results since there are not controlled vocabularies in use—not like in libraries. This search for "Delia Owens" in Amazon Books yielded a results list in which the first hit was for a book by Mark James Owens and Cordelia Dykes Owens. That, despite the fact that the query terms were "delia owens"—in quotes.

![Amazon top results "Delia Owens" in Books](https://missouri.instructure.com/courses/45003/files/7748364/preview)

### Thesaurus

In information retrieval, a _thesaurus_ of descriptors can be used as a controlled vocabulary. As with _fields_ and _browse_, _thesaurus_ can mean a lot of different things in LIS, but luckily, it only means one thing in IR!

Wikipedia tells us the following about thesauri used in IR databases, and about the information professionals who use them when carrying out organization of information.

Thesaurus (information retrieval) [https://en.wikipedia.org/wiki/Thesaurus\_(information\_retrieval)](https://en.wikipedia.org/wiki/Thesaurus_(information_retrieval)):

> In the context of [information retrieval](https://en.wikipedia.org/wiki/Information_retrieval "Information retrieval"), a **thesaurus** (plural: "thesauri") is a form of [controlled vocabulary](https://en.wikipedia.org/wiki/Controlled_vocabulary "Controlled vocabulary") that seeks to dictate semantic manifestations of [metadata](https://en.wikipedia.org/wiki/Metadata "Metadata") in the indexing of content objects. ...  
> A thesaurus serves to guide both an indexer and a searcher in selecting the same preferred term or combination of preferred terms to represent a given subject. [ISO 25964](https://en.wikipedia.org/wiki/ISO_25964 "ISO 25964"), the international standard for information retrieval thesauri, defines a thesaurus as a “controlled and structured vocabulary in which concepts are represented by terms, organized so that relationships between concepts are made explicit, and preferred terms are accompanied by lead-in entries for synonyms or quasi-synonyms.”

_Thesaurus_ is definitely one of those terms that means a lot of things to a lot of different people. For now, understand that thesauri are used to support information retrieval in databases, and the descriptors are controlled vocabulary terms that information professionals use in organizing content.

Revisit the ERIC database example and consider the tab labeled "thesaurus" above the search box: [https://eric.ed.gov/ ](https://eric.ed.gov/)

Users know the correct descriptor by first searching the thesaurus for the idea they are researching, and then they launch queries using the descriptors in order get a better, more precise result set. 

### ![](https://missouri.instructure.com/courses/45003/files/7748329/download)  
**Now This**

*   Look at the thesaurus for the ERIC database: [https://eric.ed.gov/?ti=all](https://eric.ed.gov/?ti=all)
*   Which descriptor would you choose if you wanted to help a patron wanting articles on "[Racial Prejudice](https://eric.ed.gov/?ti=Racial+Prejudice)"?

**NOTE:** _This is VERY tricky, because [Racial Prejudice](https://eric.ed.gov/?ti=Racial+Prejudice) is not a descriptor!_
<!-- #endregion -->

```python id="IU8wm6bUu9Vf"

```
