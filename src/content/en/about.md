# Tracking data on the COVID-19 spread in Slovenia

*The **"Covid-19 Tracker Slovenia"** project collects, analyses and publishes data on the spread of the SARS-CoV-2 coronavirus, the cause of COVID-19, in Slovenia. We wish to give the public a better overview of the magnitude of the issue and a proper assessment of the risk.*

## Why are we collecting this data?

In the experience of those countries where the spread of the virus has been most effectively curbed, correctly collected, up-to-date and transparently published data is vital for the effective response of public healthcare systems.
Only then the published data can stand as the basis for understanding of what is happening, for the active self-protective behaviour of people and for accepting the urgency of the safety measures taken.
Data is collected from various publicly avalilable sources, and since Saturday, March 28, we also have a direct connection with healthcare institutions and the National Institute of Public Health ([NIJZ](https://www.nijz.si/en)). They share with us structured data, which is then validated and shaped into a format suitable for visualization to be presented to the public as well as for further work in model development and forecasting. As data published in the media and certain other sources may sometimes be vague and inconsistent, the table also includes notes on sources and deductions based on incomplete data.

## What data are we collecting?

The following data from the NIJZ and various public sources is included in database on a daily basis (with history):

-   number of tests performed and number of confirmed infections

-   number of confirmed infections by category: by age, gender, region and municipality

-   hospital records for patients with COVID-19: hospitalized, in the intensive care unit (ICU), in critical condition, discharged from hospital care, recovered

-   monitoring of individual cases, particularly those in critical activities: working in healthcare, senior citizens’ homes, civil protection

-   healthcare system capacity: number of beds, intensive care units, respirators for ventilation...

    We are also constantly striving to add new important categories.
    All data is collected and available in the form of [CSV files, REST API and Google Docs Sheets](/en/data).


<details>
  <summary>How is the data edited and verified?</summary>

The database is updated with the NIJZ data (by category). The data by region and age is sometimes updated subsequently and cross-checked as the data may change as a result of epidemiological research.

Municipalities are tracked in [the Places table](https://docs.google.com/spreadsheets/d/1N1qLMoWyi3WFGhIpPFzKsFmVE0IwNP3elb_c18t2DwY/edit#gid=598557107).
Updating the hospital care data – the Patients table process:

-   All hospital announcements for COVID-19 are monitored (University Medical Centre Ljubljana, University Medical Centre Maribor, University Clinic Golnik, Celje General Hospital) – around 2pm.

-   The number of hospitalizations monitored: all departments, hospitalizations in intensive care units, and patients in critical condition.

-   Transitions (admissions/discharges) between individual conditions are also recorded (when detectable from the data).

-   Where the transition data (admission/discharge) is incomplete, the values are determined by means of deduction (using a formula).

-   All sources and deductions are recorded as comments in individual cells (possibility of verification).

-   The data is compared with the summary data on hospitalized patients and patients in intensive care published daily by the Government of the Republic of Slovenia at 11:59 pm.


</details>

## Use of the data

The data is used for various visualizations and statistics, such as [charts, infographics and maps with information on confirmed infections and hospitalized patients](/en/stats) on our own website.
Our data is also freely avaliable and is already used by other portals and projects.

<details>
  <summary>Disclaimer of responsibility (click for more)</summary>

**Please note: The information published on our site, including links to models and other sites to which we are not directly connected, is prepared with the utmost care, using available sources of data, knowledge, methodologies and technologies, in accordance with scientific standards. We believe that the visualizations and models can help explain the various factors behind the spread of the virus, including the impact of the safety measures taken and of possible future measures. Through this, we wish to emphasize that we all play an important role in this pandemic. Nonetheless, we cannot fully guarantee the accuracy, completeness or usefulness of the information on these sites, and we explicitly disclaim any responsibility for further interpretations and simulations which cite our visualizations as a source.*

</details>

## Lend a helping hand – to us, yourself and others

The project was initiated by [Luka Renko](https://twitter.com/LukaRenko) who began collecting data in the begining of COVID-19 epidemiy and has grown steadily into a team of 20 to 45 volunteers and active participants due to increasing need for data input and verification, as well as programming. It is a crowdsourcing project, supported by massive voluntary participation, where everyone can contribute with their resources or data to the best of their ability.

Do you have a suggestion, would like to help with organising the data or contribute to the project code? Please [send us a message](mailto:info@sledilnik.org) or join our [Slack](https://sledilnik.slack.com). Join in and lend a helping hand!

## Terms of use

Use and collaboration are desired: the data is collected from sources in the public domain and can be freely used, edited, processed or incorporated into any non-marketable content if citing the source – covid-19.sledilnik.org.
To export data to other formats, or use for visualization use please contact us at info@sledilnik.org.

Use of Sledilnik would not be possible without some external web services:

- CloudFlare, which helps us deliver the data to our users reliably and securely, using cookies as [described on their website](https://developers.cloudflare.com/fundamentals/get-started/reference/cloudflare-cookies/) and respecting the [privacy policy](https://www.cloudflare.com/privacypolicy/).
- Stripe, which we use to collect [donations](/en/donate) using credit cards. See [Stripe's privacy](https://stripe.com/privacy) and [cookie policy](https://stripe.com/legal/cookies-policy).
- Google fonts API, which doesn't use cookies, but [may affect user privacy](https://developers.google.com/fonts/faq#what_does_using_the_google_fonts_api_mean_for_the_privacy_of_my_users).

## Protection of personal data
The Tracker Slovenia Scientific Society (Znanstveno društvo Sledilnik) endeavours to publish only information that cannot be linked to a specific or identifiable person or that has been previously anonymised in such a way that the data subject is no longer specific or identifiable (so-called anonymised information). We strive to achieve this by only publishing information that originates from publicly available official sources and that has previously been assessed by the relevant public authority (e.g. NIJZ, MZ, MIZŠ, etc.) as sufficiently anonymised to be suitable for public release. Furthermore, additional anonymisation measures are applied to certain graphs and visualisations, such as grouping data into larger groups or presenting average values. We believe that the published information does not constitute personal data.

If you believe that the published information nevertheless constitutes personal data about you, we encourage you to contact us by email at info@sledilnik.org and in accordance with the provisions of Section III - Rectification and erasure of the General Data Protection Regulation (GDPR), to request the rectification, erasure or restriction of the processing of your personal data, to object to processing or to request access to your personal data. When doing so, please indicate as precisely as possible to which graph or visualisation or to which information your request relates. We would also like to inform you that in this case you have the right to submit a complaint with the Information Commissioner, who can be contacted by e-mail at gp.ip@ip-rs.si.

More information
- Contact details: Znanstveno društvo Sledilnik, Celovška cesta 111, 1000 Ljubljana, info@sledilnik.org
- Purpose of publishing information: As stated at the top of the page, under the section "Why".
- Legal basis: Article 39 (Freedom of Expression) of the Constitution of the Republic of Slovenia (Freedom of expression of thought, freedom of speech and public appearance, freedom of the press, and other forms of public communication and expression shall be guaranteed. Everyone may freely collect, receive, and disseminate information and opinions. Except in such cases as are provided by law, everyone has the right to obtain information of a public nature in which he has a well founded legal interest under law.)
- Data source: publicly available information provided by public institutions, as indicated in each graph or visualisation.

## Covid-19 Tracker Team

COVID-19 Sledilnik in an open source project that would not be possible without the hard work of the community members as well as numerous suggestions, comments and contributions from other people. THANK YOU!

Project collaborators:

-   [Aleks Jakulin](https://twitter.com/aleksj) - modeling, sources
-   [Aljaž Vindiš](https://vindis.io/) - infographics design
-   [Ana Slavec](https://twitter.com/aslavec) - surveys, analysis, content
-   [Andraž Vrhovec](https://github.com/overlordtm) - web page, infrastructure
-   [Andrej Srakar](http://www.ier.si/) - sources, modeling
-   [Andrej Viršček](https://udomacenastatistika.wordpress.com/author/vandrej/) - modeling
-   [Anže Voh Boštic](https://podcrto.si/author/anze/) - sources, source validation, modeling
-   [Barbara Krajnc](https://twitter.com/bakrajnc) - content, communication
-   [Bojan Košir](https://twitter.com/BojanKosir) - data model and validation, sources
-   [Boštjan Špetič](https://www.igzebedze.com/) - data scraping, communication
-   [Branko Jevtić](https://www.bananica.com/) — graphics design, web page
-   [Darja Potočan](http://www.marsowci.net/) - social networks, sources
-   [Demjan Vester](https://github.com/VesterDe) - web page
-   [Dunja Fabjan](https://twitter.com/denebdulfim) - newsletter
-   [Eva Matjašič](https://github.com/Blonduos/) - web page
-   [Eva Zupan Horaček](https://www.instagram.com/evasardinasta/?hl=en) - infographics design
-   [Gašper Mramor](https://www.linkedin.com/in/gaspermramor) - data model and validation, sources
-   [Grega Milčinski](https://www.linkedin.com/in/gregamilcinski/) - sources, data validation
-   [Igor Brejc](https://twitter.com/breki74) - visualisations
-   [Igor Kolar](https://twitter.com/igorkolar) - data model, open data
-   [Jaka Daneu](https://github.com/jalezi) -  data scraping, web page
-   [Jana Javornik](https://twitter.com/JanaSvenska) - content, sources
-   [Janez Gorenc](https://si.linkedin.com/in/janez-gorenc-03415868) - translations
-   [Janez Žibert](https://pacs.zf.uni-lj.si/janez-zibert/) - modeling coordination, SEIR model, modeling
-   [Joh Dokler](https://github.com/joahim) - visualisations, web page
-   [Jure Novak](http://jurenovak.org/) - copywriting, sources
-   [Jure Sobočan](https://www.linkedin.com/in/juresobocan) - logo, graphic design
-   [Jurij Bajželj](https://www.linkedin.com/in/bajzelj) - data model, validation, user inclusion
-   [Kaya Tokuhisa](https://www.kayatokuhisa.com) - content
-   [Luka Medic](https://www.facebook.com/luka.medic.79) - modeling, data validation, covid-spark.info
-   [Luka Renko](https://twitter.com/lukarenko) - coordination, data model and validation, visualisations
-   [Maja Pohar Perme](http://ibmi.mf.uni-lj.si/sl/o-ibmi/osebje) - modeling
-   [Maja Založnik](https://www.linkedin.com/in/maja-zalo%C5%BEnik-26034a84) - coordination, data model and validation
-   [Maks Mržek](https://www.linkedin.com/in/maks-mr%C5%BEek-98798066/) - data validation, visualisations
-   [Marko Brumen](https://twitter.com/multikultivator) - coordination, social networks, web page, contents
-   [Maruša Gorišek](https://www.linkedin.com/in/marusagorisek/) - web page, sources
-   [Matej Aleksov](https://www.linkedin.com/in/matej-aleksov/) - social networks, graphic design
-   [Matej Jurko](https://www.linkedin.com/in/matejjurko/) - sources, data validation
-   [Matej Meglič](https://www.linkedin.com/in/matejmeglic/) - coordination, data model and validation
-   [Matjaž Drolc](https://twitter.com/MatjazDrolc/) - visualisations
-   [Matjaž Lipuš](https://twitter.com/MatjazL) - sources, data validation
-   [Mia Erbus](https://github.com/miaerbus) - web page
-   [Miha Kadunc](https://twitter.com/miha_kadunc) - data model and validation, modeling
-   [Miha Markič](https://twitter.com/MihaMarkic) - REST API
-   [Milo Ivir](https://hosted.weblate.org/user/milotype/) - translations
-   [Mitja Potočin](https://github.com/mitjapotocin) - web page
-   [Nace Štruc](https://www.nace.si/) - visualisations
-   [Nejc Davidović](https://twitter.com/NejcDavidovic) - copywriting, sources
-   [Nina Rolih](https://www.facebook.com/tanoranina) - content, graphic design
-   [Nina Ružić Gorenjec](https://ibmi.mf.uni-lj.si/sl/o-ibmi/osebje) - modeling
-   [Nuša Jazbinšek]() - data model and validation
-   [Peter Keše](https://twitter.com/pkese/) - visualisations
-   [Pika Založnik]() - content, sources
-   [Sabina Tamše Kozovinc](https://www.linkedin.com/in/sabina-tamse-copywriter/) - copywriting, sources, FAQ
-   [Roman Luštrik](https://www.linkedin.com/in/roman-lu%C5%A1trik-5a6586ab) - scripting, statistics
-   [Sebastian Pleško](https://twitter.com/seba1337) - sources
-   [Sebastjan Cizel](https://sebastjancizel.github.io/) - visualisations
-   [Štefan Baebler](https://www.linkedin.com/in/stefanbaebler/) - data scraping, web page, map, translations
-   [Tanja Ambrožič]()- data validation
-   [Tomaž Kovačič](https://www.linkedin.com/in/tomazkovacic) - visualisations
-   [Vanja Cvelbar](https://github.com/b100w11) - translations
-   [Vladimir Nesković](https://www.linkedin.com/in/k35m4/) - data model, modeling
-   [Zarja Muršič](https://twitter.com/piskotk) - modeling, validation, sources
-   [Žiga Brenčič](https://zigabrencic.com) - modeling
-   [Žiga Zaplotnik](https://twitter.com/ZaplotnikZiga) - network model, modeling
