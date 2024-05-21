User guide page
===============

.. _installation:

Dashboard overview
------------------

**Header**: Use the menu to **select a species or pathogen group** to display. Each pathogen has its own dashboard configuration that is customised to show genotypes, resistances and other relevant parameters. Numbers indicate the total number of genomes and genotypes currently available in the selected dashboard. 


**Map**: Use the menu on the right to **select a variable to display per-country summary data** on the world map. Prevalence data are pooled weighted estimates of proportion for the selected resistance or genotype. Use the **filters on the left** to recalculate summary data for a specific time period and/or subgroup/s (options available vary by pathogen). A country must have N≥20 samples (using the current filters) for summary data to be displayed, otherwise it will be coloured grey to indicate insufficient data. 

Filters set in this panel apply not only to the map, but to all plots on the page. **Clicking on a country in the map** also functions as a filter, so that subsequent plots reflect data for the selected country only. 



**Detailed plots**: These are intended to show country-level summaries, but if no country is selected they will populate with pooled estimates of proportion across all data passing the current filters. The heading below the map summarizes the current filter set applied to all plots, and provides another opportunity to select a focus country. Below this are a series of tabs, one per available plot. **Click a tab title to open/close the plotting area**. The specific plots displayed will vary by pathogen, as do the definitions of AMR and genotype variables (see per-organism details below). 

All plots are interactive; use the menus at the top to **select variables to display**, and whether to show **counts or percentages**. 

Each plot has a dynamic legend to the right; click on an x-axis value to display counts and percentages of secondary variables calculated amongst genomes matching that x-axis value. For example, most pathogens will have a ‘Resistance frequencies within genotypes’ plot; click a genotype to display counts and percentages of resistance estimated for each drug.

**Downloads**: At the bottom are buttons to download (1) the individual genome-level information that is used to populate the dashboard (‘Download database (CSV format)’); and (2) a static report of the currently displayed plots, together with a basic description of the data sources and variable definitions (‘Download PDF’). Please note PDF reports are not yet available for all organisms, they will be added in future updates.


Individual pathogen details
---------------------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']


