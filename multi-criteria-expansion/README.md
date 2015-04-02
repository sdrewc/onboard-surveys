multi-criteria-expansion
===============

Transit on-board surveys are typically expanded using a single criterion.  For example, survey records may be segmented by route, direction, and time of day, and each category of record will be expanded to match the observed target.  Approaching expansion in this manner may be unneccesary limiting, as it implies observed data must meet a system-wide minimum quality threshold to be considered in the expansion.

Here, we explore a less restrictive approach, inspired by the work of [Vovsha et al.](http://onlinepubs.trb.org/onlinepubs/conferences/2014/ITM/Resources/21.pdf) in the population synthesizer realm.  The goal of the approach is to find an optimal set of expansion weights that best satisfy any number of criteria.  For example, observed targets of ridership segmented by route, direction, and time-of-day could be included alongside a system-wide observed ridership target, alongside a set of targets of ridership segmented by route, direction, and boarding location, and so on.  The goal is to create a generalizeable framework in which all available information can inform expansion weights, with subjective assessments of the importance of meeting each weight informing the optimization.

To illustrate the approach, a mini-example is provided with a trivially-small data set.  Next, a small example with real data is provided.  In progress is a production example.  In both the small and production examples, we compare the optimization results with a conventionally-dervied set of single criterion expansion weights.
  