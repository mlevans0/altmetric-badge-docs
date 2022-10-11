Clicking on a badge
*******************
When clicked, badges lead to a page on altmetric.com that contains more information on the article specified.

By default the information pages only show these first few mentions on each service. We can co-brand the page with your logo and give your visitors a more detailed breakdown of
the conversations happening around each article - please see contact sales@altmetric.com for details.

Data attributes
***************
You can optionally customize how the badge appears by adding ``data`` attributes:

.. list-table::
    :widths: 20 80
    :header-rows: 1 

    * - Attribute
      - Description
    * - ``data-{{identifier_type}}``
      - Use this data attribute to tell the embed code which identifier to use. Supported attributes are ``data-doi`` ``data-arxiv-id`` ``data-handle`` ``data-isbn`` ``data-uri`` ``data-pmid``
    * - ``data-badge-type``
      - Use this data attribute to choose a particular style of badge (see :ref:`here <Badge types>` for a list of availalbe options).
    * - ``data-badge-popover``
      - Use this data attribute to show a popover when a user hovers over the badge.
    * - ``data-badge-details``
      - Use this data attribute to show a breakdown of the data next to donut style badges.
    * - ``data-no-score``
      - Use this data attribute to specify if a score should be displayed in the center of the donut style badges.
    * - ``data-hide-less-than``
      - Use this data attribute to specify if the badge should be hidden when the Altmetric score is less than a given number.
    * - ``data-link-target``
      - Use this data attribute to specify if a user should be brought to a new tab or window when they click on a badge.
    * - ``data-condensed``
      - Use this data attribute to show a condensed version of the badge.

Some XML based journal platforms don't allow ``data`` attributes in front end code. Don't worry! As a fallback you can also specify options as CSS classes.

If you run into this problem you can pass options to the donut by adding special CSS classes to the badge element. For example:

.. list-table::
    :widths: 50 50
    :header-rows: 1 

    * - Instead of...
      - Use class...
    * - ``data-doi='xxx'``
      - ``altmetric-doi-xxx`` e.g. ``altmetric-doi-10.5339/connect.2012.9``
    * - ``data-badge-type='donut'``
      - ``altmetric-badge-type-donut`` 
    * - ``data-badge-type='1'``
      - ``altmetric-badge-type-1`` 
    * - ``data-badge-popover='xxx'``
      - ``altmetric-badge-popover-xxx`` e.g. ``altmetric-badge-popover-left``

Here's an example:

.. raw:: html

  <div class='altmetric-embed altmetric-doi-10.5339/connect.2012.9 altmetric-badge-type-donut altmetric-badge-popover-left'></div>
  <br />

``<div class='altmetric-embed altmetric-doi-10.5339/connect.2012.9 altmetric-badge-type-donut altmetric-badge-popover-left'></div>``

Popover
*******
If you'd like a popover to appear when the user hovers over a badge you can use the ``data-badge-popover`` attribute specifying where you'd like the
popover to appear: ``left``, ``right``, ``top`` or ``bottom`` .

**Popover on left**

Hover over the donut below to show a popover to its left.

.. raw:: html

    <div data-badge-type='donut' class='altmetric-embed' data-badge-popover='left' data-doi='10.1016/S0140-6736(11)61619-x'></div>
    <br />

``<div data-badge-type='donut' class='altmetric-embed' data-badge-popover='left' data-doi='10.1016/S0140-6736(11)61619-x'></div>``

**Popover below**

Hover over the badge below to show a popover below it.

.. raw:: html

    <div class='altmetric-embed' data-badge-popover='bottom' data-doi='10.1016/S0140-6736(11)61619-x'></div>
    <br />

``<div class='altmetric-embed' data-badge-popover='bottom' data-doi='10.1016/S0140-6736(11)61619-x'></div>``

Details
*******

You can choose to display details of the attention an article has received to the right of the badge by including the ``data-badge-details`` attribute.

The details display works best with the ``medium-donut`` and ``large-donut`` badge styles.

**Medium donut**

.. raw:: html

  <div data-badge-type='medium-donut' class='altmetric-embed' data-badge-details='right' data-doi='10.1016/S0140-6736(11)61619-x'></div>
  <br />

``<div data-badge-type='medium-donut' class='altmetric-embed' data-badge-details='right' data-doi='10.1016/S0140-6736(11)61619-x'></div>``

Badge types
***********

You can specify the style of badge you'd like to embed with a ``data-badge-type`` attribute. The badge types available are listed below with examples.

.. list-table::
    :widths: 20 20 60
    :header-rows: 1 

    * - Badge type
      - Example
      - Code
    * - **Default**
      - .. raw:: html

          <div class='altmetric-embed' data-doi='10.1016/S0140-6736(11)61619-x'></div>

      - ``<div class='altmetric-embed' data-doi='10.1016/S0140-6736(11)61619-x'></div>``
    * - ``donut``
      - .. raw:: html

          <div class='altmetric-embed' data-badge-type='donut' data-doi='10.1016/S0140-6736(11)61619-x'></div>

      - ``<div class='altmetric-embed' data-badge-type='donut' data-doi='10.1016/S0140-6736(11)61619-x'></div>``
    * - ``medium-donut``
      - .. raw:: html

          <div class='altmetric-embed' data-badge-type='medium-donut' data-doi='10.1016/S0140-6736(11)61619-x'></div>

      - ``<div class='altmetric-embed' data-badge-type='medium-donut' data-doi='10.1016/S0140-6736(11)61619-x'></div>``
    * - ``large-donut``
      - .. raw:: html

          <div class='altmetric-embed' data-badge-type='large-donut' data-doi='10.1016/S0140-6736(11)61619-x'></div>

      - ``<div class='altmetric-embed' data-badge-type='large-donut' data-doi='10.1016/S0140-6736(11)61619-x'></div>``
    * - ``1``
      - .. raw:: html

          <div class='altmetric-embed' data-badge-type='1' data-doi='10.1016/S0140-6736(11)61619-x'></div>

      - ``<div class='altmetric-embed' data-badge-type='1' data-doi='10.1016/S0140-6736(11)61619-x'></div>``
    * - ``4``
      - .. raw:: html

          <div class='altmetric-embed' data-badge-type='4' data-doi='10.1016/S0140-6736(11)61619-x'></div>

      - ``<div class='altmetric-embed' data-badge-type='4' data-doi='10.1016/S0140-6736(11)61619-x'></div>``
    * - ``bar``
      - .. raw:: html

          <div class='altmetric-embed' data-badge-type='bar' data-doi='10.1016/S0140-6736(11)61619-x'></div>

      - ``<div class='altmetric-embed' data-badge-type='bar' data-doi='10.1016/S0140-6736(11)61619-x'></div>``
    * - ``medium-bar``
      - .. raw:: html

          <div class='altmetric-embed' data-badge-type='medium-bar' data-doi='10.1016/S0140-6736(11)61619-x'></div>

      - ``<div class='altmetric-embed' data-badge-type='medium-bar' data-doi='10.1016/S0140-6736(11)61619-x'></div>``
    * - ``large-bar``
      - .. raw:: html

          <div class='altmetric-embed' data-badge-type='large-bar' data-doi='10.1016/S0140-6736(11)61619-x'></div>

      - ``<div class='altmetric-embed' data-badge-type='large-bar' data-doi='10.1016/S0140-6736(11)61619-x'></div>`` 

Events
******
There are two custom JavaScript events that can be fired by the badge:

* ``altmetric:show`` is fired when a badge is shown;
* ``altmetric:hide`` is fired when a badge is hidden (e.g. if its score is 0 and the data-no-score attribute is set).

These events are attached to the ``.altmetric-embed`` container, so it is possible to attach event listeners and act on them.

For example: using jQuery, one can show an alert whenever a badge is shown with the following code:

.. code-block ::

  $(function () {
      $('div.altmetric-embed').on('altmetric:show', function () {
          alert('Altmetric badge shown!');
      });
  });