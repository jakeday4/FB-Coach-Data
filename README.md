# Football Coach Data
Jake Day

### Background & General Information:

This repository includes data on the career histories of 340 Division
I - FBS college football coaches sampled during the 2009 season. The
data also include prospective data on the same coaches’ careers through
the 2015 season. The retrospective career history data were analyzed for
my
[dissertation](https://repository.lib.ncsu.edu/items/803be265-05c7-42e2-8375-1a857ddc9f67)
and two published papers:

Day, Jacob C. 2015. “Transitions to the Top: Race, Segregation, and
Promotions to Executive Positions in the College Football Coaching
Profession.” Work and Occupations 42 (4): 408–46.
https://doi.org/10.1177/0730888415580651.

Day, Jacob C. 2018. “Climbing the Ladder or Getting Stuck: An Optimal
Matching Analysis of Racial Differences in College Football Coaches’
Job-Level Career Patterns.” Research in Social Stratification and
Mobility 53 (February):1–15. https://doi.org/10.1016/j.rssm.2017.11.001.

Here is how I described the data collection in Day (2018):

> Data on 340 full-time college football coaches were gathered via a
> random cluster sample of roughly 25% of the teams (three to four) in
> each of the 11 FBS conferences and one out of three FBS independent
> programs (i.e. not conference affiliated) during the 2009 college
> football season. This produced a sample of 34 different programs
> across the nation from which career histories were compiled for each
> of the ten full-time coaches working for each program.

The prospective data was collected in 2015 when my graduate teaching
assistant and I collected prospective career data on every coach in my
original dissertation data. The motivation for collecting this
prospective data was, in part, to start correcting for one of the
fundamental flaws of my dissertation (and the papers to come out of
it)–“[survivorship
bias](https://en.wikipedia.org/wiki/Survivorship_bias).” Because I
collected retrospective career histories, I only had data on coaches who
had survived and/or were successful in their careers up to that point
(coaches in the data were at different stages of their careers). I did
not have data on coaches who had not survived or had yet to experience
success (e.g., a coach who tried to break in as graduate assistants for
a couple years and then quit or had not yet reached the upper echelons
of the college football coaching profession). One of the potential
benefits of collecting subsequent career information is that I would
have prospective data on a random cluster sample of coaches from the
2009 season. The prospective data has never been analyzed for
publication.

### Included Files

This repository contains 3 files:

1)  A person-period csv data file: “coachpp2015.csv”

2)  A codebook describing the variables within the data:
    “coachpp2015_codebook.html”

3)  The README file you are currently reading.

You can view the source material (e.g., media guides and website
biographies) from which I constructed the career history data at the
following links:

[2009_Media-Guide-Biographies](https://www.dropbox.com/scl/fo/awcznf0v1cfkxdsmk7m6j/AKTmYLD8GYkvnnZhPFU9a7w?rlkey=st0yjzokbxkicgb8jqv1iir9q&st=b2q5wgqi&dl=0)

[2015_Media-Guide-Biographies](https://www.dropbox.com/scl/fo/c991buxdprobmfb5qg7ny/AMLOxINk1llEZf0Mh1CA3rs?rlkey=yzlaeb8unn5iie8s8zvjx8tym&st=343oxlkw&dl=0)

### Measurement Details

The codebook should provide the details necessary to understand the data
but there are a couple of details worth mentioning here:

- I included variables at the finest grain possible in order to provide
  more detailed career history information than was utilized in the
  published papers cited above. I was never completely comfortable with
  the data reduction techniques I employed in those papers; including
  collapsing coaching positions into four categories based on their
  “centrality” and hiearchy (e.g., executive, central, non-central,
  peripheral), collapsing distinct playing positions into the central
  vs. non-central dichotomy, and even collapsing potentially distinct
  career trajectories into “types” via optimal matching and clustering
  techniques. To the extent my original results are sensitive to some of
  these coding decisions, the more fine grained measurement should allow
  one to examine this (I myself plan to do this when I can find the
  time).

- I also included variables (`p1` - `p8`) that indicate every position I
  originally coded from coaches’ media guide biographies. Sometimes a
  coach’s position for a given season will not be `p1` but one of the
  other `p#` variables. This has to do with how I originally collected
  the data in a wide format with the range of seasons they were at a
  given program and the range of seasons they occupied specific
  positions in that program. In the papers I published, I ended up
  creating a “hierarchical” position indicator, essentially taking their
  most central and/or hierarchical position at each program/team. But
  some coaches held multiple positions during the same season. For
  example, some head coaches also serve as offensive or defensive
  coordinators. Some offensive coordinators often serve as quarterbacks
  coaches during a season. These “extra” positions are often more
  administrative roles or title bumps (e.g., “Recruiting Coordinator”,
  “Associate Head Coach”). In looking back at the published articles, I
  don’t think I was clear about this detail of my measurement. Perhaps
  these multi-position variables can be used for sensitivity checks or
  analyzed on their own. My sense is that certain administrative or
  support positions (e.g., “analyst”, “quality control”, etc.) have
  increased in recent years and perhaps these data capture the beginning
  of this trend.[^1]

- The primary website from which I gathered the “performance”
  measures–[College Football Data
  Warehouse](https://en.wikipedia.org/wiki/College_Football_Data_Warehouse)–is
  no longer active. As I recall, I included subsequently “vacated” wins
  (e.g., due to NCAA infractions) in the `wins` variable. My thinking
  was that winning (or losing) on the field was likely more important to
  coaches’ immediate career prospects and that by the time many “wins”
  were vacated, coaches may have already moved on from that particular
  program.

- Consistent with the R statistical programming language, `NA` values
  indicate missing data.

Please don’t hesitate to reach out at jakeday4@gmail.com if you have any
questions or find any issues with the data.

### License Information

[![CC BY
4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by/4.0/)

This work is licensed under a [Creative Commons Attribution 4.0
International License](http://creativecommons.org/licenses/by/4.0/).

[![CC BY
4.0](https://i.creativecommons.org/l/by/4.0/88x31.png)](http://creativecommons.org/licenses/by/4.0/)

[^1]: I also have data on potential multiple playing positions (not
    included here), but this is less common. By the time athletes reach
    college, most of them are specializing in a particular position,
    even as they move across different levels of competition (e.g.,
    college to professional).
