Introduction
************
In this documentaion you'll find instructions for embedding Altmetric badges into your website. The badges are free to use for **academic** repositories and **individual** researchers.

If you want to use the badges on a site that isn't your lab or personal homepage, blog or an institutional repository then you should first contact us at support@altmetric.com so that we can review your use case.

.. warning:: 
    
    Do not use the badges commercially - on a journal, search engine, in an app etc. - without first talking to us! We're required by some of our data sources to keep track of who is using
    the badges and what for, and so need to issue you a license.

If you're an organisation or publisher and would like to use these badges, please `get in touch <mailto:info@altmetric.com>`_ to discuss implementation.

Quick start
***********
For researchers and academic repositories, the badges are simple to set up with a two step process:

1. Add the following line of code anywhere on an HTML page:

``<script type='text/javascript' src='https://d1bxh8uas1mnw7.cloudfront.net/assets/embed.js'></script>``

2. Add a ``div`` element specifying a `DOI <http://crossref.org/>`_ (digital object identifier), `arXiv ID <http://www.arxiv.org/>`_, 
`Handle <https://en.wikipedia.org/wiki/Handle_System>`_, `PubMed ID <https://en.wikipedia.org/wiki/PubMed#PubMed_identifier>`_, 
`ISBN <https://en.wikipedia.org/wiki/International_Standard_Book_Number>`_, URI or Altmetric ID wherever you want a badge to appear:

``<div class='altmetric-embed' data-badge-type='donut' data-doi="10.1038/nature.2012.9872"></div>``

Replace the contents of ``data-doi`` with the DOI of the article you want the badge to represent: alternatively you can use a ``data-arxiv-id`` attribute containing an arXiv ID, ``data-handle`` attribute
containing a Handle, ``data-isbn`` attribute containing an ISBN, ``data-uri`` attribute containing a URI or ``data-pmid`` attribute containing a PubMed ID.

If it isn't possible for you to set the ``data`` identifier attribute you can leave it empty and the embed script will look for a DOI in the ``dc:identifier`` or ``citation_doi`` ``<meta>`` tags of the current page. 
`Contact us <mailto:support@altmetric.com>`_ if you need any help with this.

That's it! You'll end up with a badge that looks like this:

.. raw:: html
        
    <div class='altmetric-embed' data-badge-type='donut' data-doi="10.1038/nature.2012.9872"></div>
    <br />

You can customize how the badge :ref:`looks <Badge types>`, add :ref:`popovers <Popover>` or display a breakdown of where an article has been :ref:`mentioned <Details>` by customising the embed. See  for more information :ref:`Customizations <Clicking on a badge>`.

Please see our `full terms and conditions <https://www.altmetric.com/altmetric-free-tools-terms-of-use/>`_ for more information.

Technical information
*********************
Altmetric badges are delivered by `Cloudfront <https://aws.amazon.com/cloudfront/>`_ where possible so latency should be very low.

The embed script becomes active **after** the page DOM has loaded and looks for elements with the ``altmetric-embed`` class and a related ``data-{{identifier_type}}`` identifier attribute. 
You can see a full list of supported identifier types :ref:`here <Data attributes>`.

If you're adding Altmetric badges to the DOM **after** the page has loaded (via AJAX, for example) then you can ask the Altmetric embed script to search the page again for new matches by
calling the ``_altmetric_embed_init`` function in Javascript:

.. code-block ::

    <script type='text/javascript'>
        _altmetric_embed_init();
    </script>

If you only want to load Altmetric badges from a specific container (e.g. a new ``div`` containing several elements with the ``altmetric-embed`` class loaded via AJAX) rather than searching the whole page,
you can pass an element or a string selector as a "context" argument to ``_altmetric_embed_init``:

.. code-block ::

    <script type='text/javascript'>
        _altmetric_embed_init(document.getElementById('new-container'));
        _altmetric_embed_init('#new-container');
    </script>