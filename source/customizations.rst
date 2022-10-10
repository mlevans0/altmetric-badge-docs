Clicking on a badge
*******************
When clicked the badges lead to a page on altmetric.com that contains more information on the article specified.

By default the information pages only show these first few mentions on each service. We can co-brand the page with your logo and give your visitors a more detailed breakdown of
the conversations happening around each article - please see our services for publishers page or contact sales@altmetric.com for details.

Data attributes
***************
You can optionally customize how the badge appears by adding data attributes:

.. list-table::
    :widths: 20 80
    :header-rows: 1 

    * - Attribute
      - Description
    * - ``data-badge-type``
      - Use this data attribute to choose a particular style of badge (see here for a list of options).
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
    * - ``data-condensed attribute``
      - Use this data attribute to show a condensed version of the badge.

.. warninig:: 

    Some XML based journal platforms don't allow ``data-*`` attributes in front end code. Don't worry! As a fallback you can also specify options as CSS classes.

You can read more about this here.

Build your own
**************

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
  
  As a reminder: if you want to use the badges on a site that isn't your lab or personal homepage, blog or an institutional repository then you should first contact us at support@altmetric.com
  so that we can clear your use case. Do not use the badges commercially - on a journal, search engine, in an app etc. - without talking to us first!


********