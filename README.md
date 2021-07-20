
# PyPlutchik
Python visualisation for Plutchik annotated corpora.

PyPlutchik is a module for visualizing the emotional fingerprint of corpora and text annotated with the [Plutchik's model of emotions](https://en.wikipedia.org/wiki/Robert_Plutchik).

PyPlutchik provides a plug-and-play tool for a quantitative representation of Plutchik's emotions in a text or corpus. It is respectful of original colors and spatial displacement of each petal in the Plutchik's wheel.
In Pyplutchik users can just pass a dictionary as only parameter, where dictionary's keys must be the 8 basic emotions. Each value must be ∈ [0, 1].

<img src="https://github.com/alfonsosemeraro/pyplutchik/blob/master/img/example01.png" alt="Example 1" width="650"/>



Users can represent also the three degrees of intensity for each emotion, just by providing a 3-dimensional iterable as value for each key in the dictionary. Each 3-dimensional value must sum somewhere between 0 and 1.

<img src="https://github.com/alfonsosemeraro/pyplutchik/blob/master/img/example02.png" alt="Example 2" width="650"/>



PyPlutchik also represents primary dyads, secondary dyads, tertiary dyads and opposite emotions. It automatically understand what kind of dyad users want to display from the dictionary's keywords.

<img src="https://github.com/alfonsosemeraro/pyplutchik/blob/master/img/example03.png" alt="Example 3" width="650"/>




Integration with _matplotlib_ is easy, so PyPlutchik can be used for also for composed plots.

<img src="https://github.com/alfonsosemeraro/pyplutchik/blob/master/img/dyads_show.png" alt="Full spectrum of emotions" width="500"/>


### A couple tricks

One can focus on a subset of emotions, ignoring the remaining ones...

<img src="https://github.com/alfonsosemeraro/pyplutchik/blob/master/img/highlight_emotions.png" alt="Highlight some emotions" width="500"/>


... or can hide coordinates, ticks and labels, plotting only the petals of the flower

<img src="https://github.com/alfonsosemeraro/pyplutchik/blob/master/img/imdb_full.png" alt="Small multiple" width="500"/>


