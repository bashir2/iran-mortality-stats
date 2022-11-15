
__[NOTE: This is a work in progress shared for better collaboration.]__


For a summary of this in Persian, see [this thread](https://twitter.com/BashirSadjad/status/1591752026610102272),
or [the unrolled version](https://threadreaderapp.com/thread/1591752026610102272.html).


# What is this?

The is a [notebook](iran_mortality_stats.ipynb) for analyzing official numbers of registered deaths
around November 2019 in Iran. The core question is how much of the
significant excess rate (compared to previous years or months before/after) 
is possibly due to the brutal crackdown of protests in "Bloody November"?
And how much might be due to other causes.

## Background and context

The [Bloody November](https://en.wikipedia.org/wiki/2019%E2%80%932020_Iranian_protests) (in Persian آبان خونین), refers to a 
series of protests that were sparked after the price of fuel was tripled
suddenly on 15 November 2019. During a few days of widespread protests, the
Iranian security forces used live ammunition to kill hundreds or maybe more than a thousand of protesters. Amnesty International has identified at least
[321 deaths](https://www.amnesty.org/en/documents/mde13/2308/2020/en/),
in a series of reports that were updated during the two years after that bloody event (gradually identifying more victims).

In December 2019, [Reuters reported](https://www.reuters.com/article/us-iran-protests-specialreport/special-report-irans-leader-ordered-crackdown-on-unrest-do-whatever-it-takes-to-end-it-idUSKBN1YR0QR)
that as many as 1500 people were killed when the supreme leader,
Ali Khamenei, ordered the security apparatus to
_"do whatever it takes to end it"_. Reuters declared
_"three Iranian interior ministry officials"_ as the source for this number; it also said that this figure includes members of security forces
too. US government's [estimate](https://www.nbcnews.com/news/world/u-s-says-iran-may-have-killed-1-000-protesters-n1096666)
is that more than 1000 protesters were murdered.

Official seasonal mortality rate statistics that were first examined to
determine the real impact of COVID-19 in Iran, revealed that Fall 2019
has had an unusually higher death rate compared to previous years (e.g.,
[here](https://kavehmadani.medium.com/in-search-of-the-murder-making-sense-of-irans-reported-deaths-4279d2b03175)
is a report of 9488 extra deaths compared to Fall 2018).
Later analysis for monthly mortality stats, revealed that Aban 1398
(23 Oct. 2019 to 22 Nov. 2019) had over 4000 extra deaths compared to
the months before and after it and more than 6000 extra deaths compare
to the same period of the previous year
([source](https://www.radiofarda.com/a/commentary-on-death-toll-report-of-november-2019/31276714.html)).

In this notebook we look at the weekly mortality stats that were released
a while ago (I think, sometime in Summer 2021). The main goal here is to
collect various pieces of evidence available in one place to make it
easier for others to conduct more investigations.
Obviously, in a normal society, the exact number of victims of police
brutallity should be announced by official authorities and each case
fully investigated. In the absence of such investigations, we are
left with whatever is available to us to shed some light on the possible
extent of this massacre and to seek some explanation and accountability.

## The structure of this "notebook"
The main data is the weekly death stats released by National Organization 
for Civil Registration (NOCR) available [here](https://www.sabteahval.ir/Page.aspx?mId=49826&ID=3273&Page=Magazines/SquareshowMagazine), plus
some othre related data linked throughout the notebook.
Each section looks at the data from a different angle, e.g., some sanity
checks, plotting and comparing with previous years, looking at the
distribution of location, age and cause of death, comparison with
Canada trends, etc.

One may question the authenticity of NOCR's data, especially when it comes
to age, location, and cause of death data; but our approach here is to
treat the data as authentic to see what else can be inferred from it.
This is clearly a work in progress and by no means a thorough analysis.
A lot of further statiscial analysis can be done on this (e.g.,
some ARIMA modeling); and BTW I am not a statistician!
These are all to say that forking this work and more contributions are welcome.

Finally, a lot of data processing scripts below
can be improved for better readability, performance, etc.; optimizing
those aspects has not been the goal. The runtime environment is
[Google Colab](https://colab.research.google.com/).

Bashir Sadjad, Winter 2021 (1400)

[minor updates Nov. 2022; Aban 1401].
