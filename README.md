# Automatic sentiment analysis of Fed and ECB protocols

In this project a machine learning approach is implemented and applied for
analyzing meeting minutes of the [Federal Open Market Committee (FOMC)](https://www.federalreserve.gov/monetarypolicy/fomc.htm), as well
as of the [Governing Council of the European Central Bank (ECB)](https://www.ecb.europa.eu/ecb/orga/decisions/govc/html/index.en.html). Both institutions
hold eight regular meetings per year. The related minutes contain detailed summaries
of discussed topics in the meeting and are released three to four weeks after the corresponding meeting took place.
Minutes are provided publicly by the Federal Open
Market Committee1 and the Governing Council of the European Central Bank2.

Analogous to the paper of [Jegadeesh and Wu (2015)](https://www.researchgate.net/publication/318004818_Deciphering_Fedspeak_The_Information_Content_of_FOMC_Meetings)
the minutes of each meeting
are divided into individual paragraphs which are assigned to distinct economic topics
using a [Latent Dirichlet Allocation (LDA)](http://www.jmlr.org/papers/volume3/blei03a/blei03a.pdf) algorithm. Furthermore, net tone and
uncertainty level of each topic and meeting are extracted. While Jegadeesh
and Wu (2015) only considered a time frame from June 1991 until December 2012, this
thesis extends the observation period to recent days. 

The Governing Council of the
European Central Bank started to publish similar minutes on February 2015. 
Therefore, the database for the ECB is much smaller than the one of the FOMC.
In analyzing proportion, net tone and uncertainty of different topics in the minutes
over time a qualitative view on the work of central banks is taken. 

The main idea behind this approach is to identify additional qualitative information being released
in minutes besides quantitative data like federal funds target rates. Even if the minutes of each meeting are released about a few weeks after, Jegadeesh and Wu (2015)
show that it still contains some additional information content based on the superior
information of central banks. The analysis of the content of these soft data creates a
certain transparency in the intentions and knowledge of central banks
