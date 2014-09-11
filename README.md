# Seay Music Library Catalog at Colorado College 

This repository contains the source code for the Music Library Catalog 
Enrichment Project with the following project goals:

*   RDA Enhancement of Existing MARC Records

    Using the latest (February 2013) report, 
    [PCC Post-Implementation Hybrid Bibliographic Records Guidelines Task Group][PPC_HYBRID], 
    all MARC records for material that is in the Music Library will be processed according the
    their recommended conversion guidelines starting on page 19. 

    Additional RDA conversions will be developed in consultation with the Sealy Library 
    Librarian and Staff. 

    Future iterations could include more RDA-specific enhancements through using 
    [RDA Vocabularies][RDA_VOCAB] in conjunction with [BIBFRAME] and [Schema.org][SCHEMA]
    [Fedora 4][FEDORA] Objects.
    

*   Linked Data Authority Control 

    With the growth of Discovery Layers for collections, more bibliographic linked data,
    and newer models of Authority entities ([BIBFRAME][BIBFRAME]) the role of Authority 
    control for bibliographic information is seeing radical changes from past processes.
    However, Colorado College still needs to maintain workflows for updating and managing
    Authority records in a legacy MARC21-based catalog.

    Using the Music Library's MARC bibliographic records, the larger Authority Records for the 
    Tutt Library Catalog TIGER, and other data sources, MARC Authority records will be 
    dynamically downloaded and updated based on Linked Data interfaces from the Library of 
    Congress [id.loc.gov][ID_LOC], OCLC sponsored [VIAF][VIAF] and their own web services, 
    along with Linked Data from other sources like the [Getty Vocabularies][GETTY_VOCAB] and
    [Discogs][DISCOGS].  

*   Song Index for Music Albums and Score Collections 

    Using both [Fedora 4][FEDORA], [Elastic Search][ES], and [Flask][FLASK], a new service for the Sealy Library will
    be created that will allow patrons to search for specific songs in albums and in musical
    scores. This Song Index will use a [BIBFRAME][BIBFRAME] and [Schema.org][SCHEMA] 
    vocabularies to capture track and song level statements that can be searched and displayed
    through a common, web catalog interface. 

    This Song Index will use the underlying semantic datastore built with Fedora 4 and Elastic 
    Search with a web front-end built using Flask.
    
[BIBFRAME]: http://bibframe.org/
[DISCOGS]: http://www.discogs.com/
[GETTY_VOCAB]: http://www.getty.edu/research/tools/vocabularies/lod/
[ES]: http://www.elasticsearch.org/
[FEDORA]: http://fedora-commons.org/
[FLASK]: http://flask.pocoo.org/
[ID_LOC]: http://id.loc.gov/
[PPC_HYBRID]: https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=0CCAQFjAA&url=http%3A%2F%2Fwww.loc.gov%2Faba%2Fpcc%2Frda%2FRDA%2520Task%2520groups%2520and%2520charges%2FPCC-Hybrid-Bib-Rec-Guidelines-TG-Report.docx&ei=onoQVImZBoqfyAS12oDIDw&usg=AFQjCNEjwl6StfvyczUd3PosbgaZwxnVww&sig2=PzaNEBlMn9COYC05vfOmRA&bvm=bv.74649129,d.aWw
[RDA_VOCAB]: https://github.com/RDARegistry/RDA-Vocabularies
[SCHEMA]: http://schema.org/
[VIAF]: http://viaf.org/
