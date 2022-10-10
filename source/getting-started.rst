Introduction
############
On this page you'll find instructions for embedding the Altmetric badges in your website. The badges are free to use for academic repositories and individual researchers.

.. note::
    If you want to use the badges on a site that isn't your lab or personal homepage, blog or an institutional repository then you should first contact us at support@altmetric.com
    so that we can clear your use case. Do not use the badges commercially - on a journal, search engine, in an app etc. - without talking to us first! 
    We're required by some of our data sources to keep track of who is using the badges and what for, and so need to issue you a license.

If you're an organisation or publisher and would like to use these badges, please `get in touch <mailto:info@altmetric.com>`_ to discuss implementation.

For researchers and academic repositories, the badges are simple to set up with a two step process:

1. Add the following line of code anywhere on an HTML page:

``<script type='text/javascript' src='https://d1bxh8uas1mnw7.cloudfront.net/assets/embed.js'></script>``

2. Add a div element specifying a `DOI <http://crossref.org/>`_ (digital object identifier), `arXiv ID <http://www.arxiv.org/>`_, 
`Handle <https://en.wikipedia.org/wiki/Handle_System>`_, `PubMed ID <https://en.wikipedia.org/wiki/PubMed#PubMed_identifier>`_, 
`ISBN <https://en.wikipedia.org/wiki/International_Standard_Book_Number>`_, URI or Altmetric ID wherever you want a badge to appear:

``<div class='altmetric-embed' data-badge-type='donut' data-doi="10.1038/nature.2012.9872"></div>``

Replace the contents of ``data-doi`` with the DOI of the article you want the badge to represent: alternatively you can use a ``data-arxiv-id`` attribute containing an arXiv ID, ``data-handle`` attribute
containing a Handle, ``data-isbn`` attribute containing an ISBN, ``data-uri`` attribute containing a URI or ``data-pmid`` attribute containing a PubMed ID.

If it isn't possible for you to set the ``data-doi`` attribute you can leave it empty and the embed script will look for a DOI in the ``dc:identifier`` or ``citation_doi`` <meta> tags of the current page. 
`Contact us <mailto:support@altmetric.com>`_ if you need any help with this.

That's it! You'll end up with a badge that looks like this:

.. raw:: html
        
        <div class='altmetric-embed' data-badge-type='donut' data-doi="10.1038/nature.2012.9872"></div>
        <br />

You can change how the badge looks, add popovers or display a breakdown of where an article has been mentioned by customising the embed - see below.

Please see our `full terms and conditions <https://www.altmetric.com/altmetric-free-tools-terms-of-use/>`_ for more information.