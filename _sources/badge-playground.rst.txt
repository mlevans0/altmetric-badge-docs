Badge generator
***************
Altmetric badges can be modified to fit the look and style of your website, so you can find a design that works for you. Try some of the options using our badge generator below!

.. raw:: html

    <div id="golden-kestrel">
        <div class="badge-builder-container">
            <div class="embed-form"></div> 
            <div class="embed-example"></div>
            <div class="embed-code-container">
              <b>The HTML to copy into your page for the above embed:</b>
              <div class="embed-code"></div>
            </div>
        </div>
    </div>
    <br />

.. tip::

  As a reminder: if you want to use the badges on a site that isn't your lab or personal homepage, blog or an institutional repository then you should first contact us at support@altmetric.com so that we can clear your use case. Do not use the badges commercially - on a journal, search engine, in an app etc. - without talking to us first!

Examples gallery
****************

**Small badge design using the DOI 10.1038/nature.2012.9872**

Click on the badge to see more information about this article.

  .. raw:: html

    <div class='altmetric-embed' data-doi='10.1038/nature.2012.9872'></div>

.. code::

  <div class='altmetric-embed' data-doi='10.1038/nature.2012.9872'></div> 

**Donut style badge using the arXiv ID 1209.4191**

Click on the badge to see more information about this article.

 .. raw:: html

    <div class='altmetric-embed' data-badge-type='donut' data-arxiv-id='1209.4191'></div>

.. code::

  <div class='altmetric-embed' data-badge-type='donut' data-arxiv-id='1209.4191'></div> 

**Donut style badge using the PubMed ID 21771119**

Click on the badge to see more information about this article.

 .. raw:: html

    <div class='altmetric-embed' data-badge-type='donut' data-pmid='21771119'></div>

.. code::

  <div class='altmetric-embed' data-badge-type='donut' data-pmid='21771119'></div>  

**Donut style badge using the Handle 2022/14471**

Click on the badge to see more information about this article.

 .. raw:: html

    <div class='altmetric-embed' data-badge-type='donut' data-handle='2022/14471'></div>

.. code::

  <div class='altmetric-embed' data-badge-type='donut' data-handle='2022/14471'></div> 

**Donut style badge using a URI**

**Legacy support only**. Please note that we no longer support URI tracking.

 .. raw:: html

    <div class='altmetric-embed' data-badge-type='donut' data-uri='http://ecancer.org/news/3182-genetic-marker-in-vitamin-d-receptor-gene-associated-with-increased-pancreatic-cancer-survival.php'></div>

.. code::

  <div class='altmetric-embed' data-badge-type='donut' data-uri='http://ecancer.org/news/3182-genetic-marker-in-vitamin-d-receptor-gene-associated-with-increased-pancreatic-cancer-survival.php'></div> 

**Donut style badge using the ISBN 978-3-319-25557-6**

Badges support both 10 and 13 digit ISBNs and do not require normalization. 

 .. raw:: html

    <div class='altmetric-embed' data-badge-type='donut' data-isbn='978-3-319-25557-6'></div>

.. code::

  <div class='altmetric-embed' data-badge-type='donut' data-isbn='978-3-319-25557-6'></div> 

**Donut style badge using the URN urn:nbn:de:hbz:294-46567**

Click on the badge to see more information about this article.

 .. raw:: html

    <div class='altmetric-embed' data-badge-type='donut' data-urn='urn:nbn:de:hbz:294-46567'></div>

.. code::

  <div class='altmetric-embed' data-badge-type='donut' data-urn='urn:nbn:de:hbz:294-46567'></div>

**Donut style badge using the NCT ID NCT01564784**

Click on the badge to see more information about this article.

 .. raw:: html 

    <div class='altmetric-embed' data-badge-type='donut' data-nct-id='NCT01564784'></div>

.. code::

  <div class='altmetric-embed' data-badge-type='donut' data-nct-id='NCT01564784'></div> 

**Donut style badge using the Altmetric ID 569975**
 
Altmetric Ids are transient and unstable over the medium term. For long term application it is recommended that persistent IDs such as DOIs, arXiv IDs or PMIDs are used instead.

 .. raw:: html

    <div class='altmetric-embed' data-badge-type='donut' data-altmetric-id='569975'></div>

.. code::

  <div class='altmetric-embed' data-badge-type='donut' data-altmetric-id='569975'></div>

**Donut style badge using Altmetric ID 569975 showing no score**

Altmetric Ids are transient and unstable over the medium term. For long term application it is recommended that persistent IDs such as DOIs, arXiv IDs or PMIDs are used instead.

 .. raw:: html

    <div class='altmetric-embed' data-no-score='true' data-badge-type='donut' data-altmetric-id='569975'></div>

.. code::

  <div class='altmetric-embed' data-no-score='true' data-badge-type='donut' data-altmetric-id='569975'></div>

**Donut style badge using the PubMed ID 21771119, clicking on the badge opens the Details Page in a new tab**

Here we're using the ``data-link-target`` attribute to specify that the Details Page for the article should open in a new tab instead of the current tab.

 .. raw:: html

    <div class='altmetric-embed' data-link-target='_blank' data-badge-type='donut' data-pmid='21771119'></div>

.. code::

  <div class='altmetric-embed' data-link-target='_blank' data-badge-type='donut' data-pmid='21771119'></div> 

**Small badge design for DOI 10.1016/S0140-6736(11)61619-x with a popover appearing to the left (hover over the badge)**

Here we're using the ``data-badge-popover`` attribute to specify that the article details should appear to the left of the badge.

 .. raw:: html

    <div class='altmetric-embed' data-badge-popover='left' data-doi='10.1016/S0140-6736(11)61619-x'></div>

.. code::

  <div class='altmetric-embed' data-badge-popover='left' data-doi='10.1016/S0140-6736(11)61619-x'></div>

**Medium style donut and including article details to the side**

Here we're using the ``data-badge-details`` attribute to specify that the articles details should be displayed to the right of the badge.

 .. raw:: html

    <div class='altmetric-embed' data-badge-type='medium-donut' data-badge-details='right' data-doi='10.1136/bmj.39471.430451.BE'></div>

.. code::

  <div class='altmetric-embed' data-badge-type='medium-donut' data-badge-details='right' data-doi='10.1136/bmj.39471.430451.BE'></div>

**Condensed article details**

Here we're using the ``data-condensed`` attribute to reduce the amount of text shown in the articles details section.

 .. raw:: html

    <div class='altmetric-embed' data-badge-type='donut' data-condensed='true' data-badge-details='right' data-doi='10.1136/bmj.39471.430451.BE'></div>

.. code::

  <div class='altmetric-embed' data-badge-type='donut' data-condensed='true' data-badge-details='right' data-doi='10.1136/bmj.39471.430451.BE'></div>

**No mentions / ghost donut**

This is an example of a badge for an article that doesn't currently have any attention.

 .. raw:: html

    <div class='altmetric-embed' data-badge-type='donut' data-doi='10.1016/S0140-6736(11)61619-x-y'></div>

.. code::

  <div class='altmetric-embed'data-badge-type='donut' data-doi='10.1016/S0140-6736(11)61619-x-y'></div> 

**Hiding the badge when the Altmetric Attention Score is less than a specified threshold**

Here we're using the ``data-hide-less-than`` attribute to prevent the badge from showing if the score is less that 100.

 .. raw:: html

    <div class='altmetric-embed' data-badge-type='medium-donut' data-hide-less-than='100' data-badge-details='right' data-doi='10.1136/bmj.39471.430451.BE'></div>

.. code::

  <div class='altmetric-embed' data-badge-type='medium-donut' data-hide-less-than='100' data-badge-details='right' data-doi='10.1136/bmj.39471.430451.BE'></div>

**Hiding a badge that has no mentions**

If ``data-hide-no-mentions`` is set then the embed won't display at all if the article hasn't been mentioned.

 .. raw:: html

    <div class='altmetric-embed' data-hide-no-mentions='true' data-doi='10.1016/S0140-6736(11)61619-x-y'></div>

.. code::

  <div class='altmetric-embed' data-hide-no-mentions='true' data-doi='10.1016/S0140-6736(11)61619-x-y'></div>

**Redirect users to a specific customized/branded Details Page**

Setting ``data-template`` to the name of a customized Detail Page's sub-domain will redirect users to that Details Page instead of to the one associated with where the badges are being hosted. In this example, clicking the bade will take you to https://dimensions.altmetric.com/details/101918214 instead of https://www.altmetric.com/details/101918214.

 .. raw:: html

    <div class='altmetric-embed' data-template='dimensions' data-doi='10.1136/bmj.39471.430451.BE'></div>

.. code::

  <div class='altmetric-embed' data-template='dimensions' data-doi='10.1136/bmj.39471.430451.BE'></div>