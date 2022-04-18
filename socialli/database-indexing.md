# Database Indexing

Aiming to structure the concept of multimedia indexing, search and retrieval, based on the data growth curve from the small, locally stored, multimedia collections to the huge, heterogeneous and context-rich social multimedia collections.

Multimedia indexing, search and retrieval is a multi-step process that deeply depends on the content type and its characteristics. The typical content-based multimedia indexing (CBMI) and retrieval methods apply the well studied query by example (QBE) paradigm, where a multimedia (MM) object is used as a query to retrieve similar multimedia objects

In our first phase we mainly focus on text and image indexing, search and retrieval, yet the concepts, workflow and conclusions are valid also for other multimedia objects such as video, audio, 3D, etc. A common initial step of multimedia indexing is the extraction of characteristic features from the content in order to describe it in a more compact and discriminative manner.

### Structure Indexing

Indexing structures are data structures that help to reduce comparisons and consequently reduce the search time. Indexing structures aims to address the problem of searching inside large collections of multimedia objects.

To enhance the accuracy and fast retrieval of the content we will be having 3 approaches to avoid the full table scans and doing various kind of indexing explained below but even in some exceptional cases where full table scans do happen multi worker threads will be configured and launched.&#x20;

* Content-based multimedia Indexing
* Event-based Indexing
* Time-related multimedia Indexing

Apart from the above mentioned indexing strategies we will have indexes for the regular structures which will be queried most frequently as per system's functionality. Adding these indexes will take a huge load off of the DB reads and writes since it would initiate bitmap heat scans of the structures which reduces the retrieval time massively.

