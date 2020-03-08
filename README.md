# COVID-19 Pandemic Forecast
by [Alex Beal](https://twitter.com/beala) and [Nick Vanderweit](https://twitter.com/nvanderw)

We are non-experts with an interest in forecasting world events. Our approach is to first determine a prior probability given past events, and update that probability with current evidence. The calculations below use the odds form of Bayes’ theorem.
# Definition of pandemic
We define a coronavirus pandemic as an event where > 10% of the world is infected by coronavirus before 2022. In this forecast, we focus on how prevalent we believe the coronavirus outbreak will become, although we use the estimated fatality rate to make some estimates about prevalence.
# Prior probability
We estimate the prior probability of a pandemic given an outbreak of this size by looking at historical cases of outbreaks of this size. Below are outbreaks of respiratory viruses causing more than 1,000 confirmed cases.

| Not Pandemic | Pandemic |
|--------------|----------|
| [MERS](https://en.wikipedia.org/wiki/Middle_East_respiratory_syndrome) (2018)  | [H1N1](https://en.wikipedia.org/wiki/Influenza_A_virus_subtype_H1N1) (2009)|
| [H1N1](https://en.wikipedia.org/wiki/2015_Indian_swine_flu_outbreak) (India, 2015): Since H1N1 had already become seasonal, it’s unclear if this ever had the potential to become a pandemic.| [London Flu](https://en.wikipedia.org/wiki/London_flu) (1972): Thousands of deaths, outbreaks in several countries, but unclear what percentage of the world it infected. |
| [SARS](https://en.wikipedia.org/wiki/Severe_acute_respiratory_syndrome) (2003)        |  [Hong Kong Flu](https://en.wikipedia.org/wiki/1968_flu_pandemic) (1968) |
| [Russian Flu](https://en.wikipedia.org/wiki/Influenza_A_virus_subtype_H1N1) (1977) | [Asian Flu](https://en.wikipedia.org/wiki/Influenza_A_virus_subtype_H2N2#Asian_flu) (1956) |
|                    | Spanish Flu (1918) |

It’s unclear if Russian Flu and the 2015 Indian H1N1 outbreak should be included, as they were both outbreaks of viruses that were either already in circulation, or had been in circulation in the past.

It’s also unclear if London Flu ever went on to infect a significant percentage of the world, or if the outbreaks across several countries were small.

It’s also true that MERS and SARS never got nearly to the size of the current outbreak. We include them because they’re the only large outbreaks to be contained in the 21st century.

**Including all instances, our prior is 5:4 odds that an outbreak of this size will become a pandemic.**

**If we exclude questionable instances (Indian H1N1, Russian Flu, and London Flu), our prior is 2:1.**

Some commenters have expressed concern about undersampling contained viruses. However these data would also undersample mild infections that spread widely e.g. known coronaviruses already in circulation that cause colds. So it is unclear to us how to update on this.

There has also been concern about what time range to consider, especially given that the data shows no non-pandemic cases for most of the 1900s. Perhaps advances in gene sequencing and other diagnostic technology give us reasons to give more weight to more recent data. Considering only cases since 2000, (SARS, MERS, and H1N1), we get a **1:2 prior**.

**Our priors range from 1:2 at the low end to 2:1 at the high end.**

# Evidence for pandemic
## Undetected cases
[Air travel data suggests that there are countries with a substantial number of undetected imported cases.](https://docs.google.com/spreadsheets/d/1-HieY7joEv0ngoBjrzVoRNGoiQMty3T_Jon7k9xfF2Q) Cambodia, for example, has a similar amount of air travel from affected areas as compared to Singapore, but only has 1 confirmed case compared to Singapore’s 22 confirmed importations. Thailand has about 4 times as much air travel from China as Singapore, but has only 23 imported cases, where we would expect around 92. If these undetected importations are causing undetected outbreaks, it may be impossible to contract trace and quarantine the ill and contain the virus.

### February 22 Update
There have been 18 confirmed cases and 4 deaths in Iran. [WHO estimates](https://www.who.int/docs/default-source/coronaviruse/situation-reports/20200222-sitrep-33-covid-19.pdf) the Infection Fatality Ratio to be in the range 0.3%-1%. Applied to Iran, this yields between 400 and 1,300 total cases. If all cases were known, the official numbers would suggest an implausibly high 4/18 ~= 22% IFR. This suggests orders of magnitude more unconfirmed cases than confirmed.

The WHO has claimed that the outbreak in Iran has not been successfully traced back to China. It’s not entirely clear to us what this implies, but it would be consistent with:

1. Cases spread from China to Iran directly, but many of the infected Iranians were not detected.
2. Cases spread undetected from an intermediate country.

Given the relatively low number of expected importations from China to Iran, case (1) implies higher numbers of importations to many other countries including Thailand, Japan, South Korea, Taiwan and the United States. For instance, the import rate to the Philippines is roughly an order of magnitude higher than to Iran, so case (1) implies many undetected cases around the world.

Case (2) also implies an outbreak in whatever intermediate country the virus was imported from. For instance, Iran’s largest trading partner for imports is the United Arab Emirates, which has almost 5 times the importation risk from China that Iran does, and has recently detected cases tracing back to China.

The aforementioned [WHO situation report](https://www.who.int/docs/default-source/coronaviruse/situation-reports/20200222-sitrep-33-covid-19.pdf) shows a sharp increase in cases outside of China, with few new cases originating in China. Two new countries (Lebanon and Israel) are reporting COVID-19 cases.

Relevant studies:
- [Report 6: Relative sensitivity of international surveillance](https://www.imperial.ac.uk/media/imperial-college/medicine/sph/ide/gida-fellowships/Imperial-College---COVID-19---Relative-Sensitivity-International-Cases.pdf): "we estimated that about two thirds of COVID-19 cases exported from mainland China have remained undetected worldwide, potentially resulting in multiple chains of as yet undetected human-to-human transmission outside mainland China."
- [Using predicted imports of 2019-nCoV cases to determine locations that may not be identifying all imported cases](https://www.medrxiv.org/content/10.1101/2020.02.04.20020495v2): This study flags Indonesia, Cambodia, and Thailand as places at risk of having undetected importations.
- [Undetected cases are likely in countries around the world, with greater risk in countries of low detection capacity and high connectivity to the epicenter of the outbreak](https://www.medrxiv.org/content/10.1101/2020.02.13.20022707v2): “Undetected cases are likely in countries around the world, with greater risk in countries of low detection capacity and high connectivity to the epicenter of the outbreak.”
- [2019 Novel Coronavirus Global Risk Assessment](http://rocs.hu-berlin.de/corona/): Up to date numbers of relative import risk based on air travel data.

**We believe this is strong evidence in favor of an eventual pandemic. This updates our prior 4:1.**

# Evidence against pandemic
## No large outbreaks outside of China
With the exception of the Diamond Princess cruise ship, there have been no large outbreaks outside of China. This is promising, but we believe this is consistent with the possibility that outbreaks are occuring undetected. It has only been 27 days since Singapore’s first detected importation. If undetected importations started occurring at about the same time in other countries, it’s possible they are still small enough to fly under the radar given the incubation period of 7 days and an R0 of 2.5.

**That said, this provides some evidence that the virus is being contained. This updates our prior 3:4.**

## The outbreak in China may be peaking
The official numbers coming out of China suggest that the outbreak inside China may be peaking. If an outbreak inside China can be contained, that’s a signal that China’s tactic of large scale quarantine is effective even with case numbers in the tens of thousands. Other countries may be able to deploy a similar tactic against their outbreaks should they occur.

That said, we have ample reason to be skeptical.

- Given the political pressures to drive down the number of cases, and the constant changing case definitions, it’s hard to be sure the trend is real. We can’t rule out disinformation given the [political climate in China](https://www.latimes.com/world-nation/story/2020-02-11/china-coronavirus-peoples-war).
- Even if cases are brought to a very low number, China must at some point end the quarantine which could lead to a second wave. China must eliminate the virus completely for this to be effective.

**We don’t see this as a likely way for the outbreak to end, but it may buy the world time to develop a vaccine, treatment, or better surveillance, so we give it a 4:5 update.**

## Development of an effective vaccine or antiviral
Given the possibility of pandemic, governments and private companies are incentivized to create vaccines and treatments. There are some potentially promising avenues:

- [Remdesivir prevents MERS coronavirus disease in monkeys | National Institutes of Health](https://www.nih.gov/news-events/news-releases/remdesivir-prevents-mers-coronavirus-disease-monkeys)
- [The coronavirus prompts a burst of clinical trials in search of a treatment](https://www.statnews.com/pharmalot/2020/02/19/coronavirus-clinical-trials-china/)
- Use of an HIV antiviral cocktail to treat the SARS coronavirus in patients: [Role of lopinavir/ritonavir in the treatment of SARS: initial virological and clinical findings.](https://www.ncbi.nlm.nih.gov/pubmed/14985565)

While we would expect to see a flurry of research into such avenues regardless of whether they were destined for success, it is not out of the question that advances in antiviral R&D for coronaviruses would produce mitigations for COVID-19. However in the world of pharmaceutical development, there is a huge difference between a promising initial trial and large-scale distribution of an effective treatment to hundreds of thousands or millions of people.

[One report](https://academic.oup.com/biostatistics/article/20/2/273/4817524) estimates that 9.6% of Phase 1 trials will eventually be deemed safe and effective. There are > 120 clinical trials happening for COVID-19, so it is possible that some of the treatments will be effective. However, we have reasons to suspect that the success rate of these trials will be lower than standard Phase 1 base rates. Due to the desperate situation in China, where the vast majority of these trials are happening, it is plausible that many clinical trials are being conducted that would not have advanced to the clinical trial stage in other circumstances. Hence we should expect a lower probability that a given trial will succeed here, assuming say 1%. Additionally, for this to reduce the chance of pandemic, the successful trial would have to be a treatment that slows or stops the spread. The treatment would have to be manufactured on a large scale and distributed to many countries with varying quality of healthcare infrastructure, and the trials, manufacture, and distribution would have to happen before the outbreak of a pandemic in order to prevent one from occurring.

Given that, in the H1N1 case, it was mere months between the first outbreaks outside of Mexico and declarations of pandemic, we think it’s very unlikely that a given treatment will arrive in time to prevent pandemic. **Our Bayesian update for this is 99:100.**

# Posterior Probability

| Prior odds | 5:4 | 2:1 | 1:2 |
|--|--|--|--|
| Undetected cases | 4:1 | | |
| No large outbreak outside of China|3:4| | |
| China outbreak peaking | 4:3 | | |
|Development of effective vaccine or antiviral | 99:100| | |
|Combined update | 297:125 ~= 2.376 | | |
| Posterior odds |297:100 ~= 75% | 594:125 ~= 83%| 297:250 ~= 54%|

# What would change our minds
## Countries that we expect to have oubreaks continue to have a low number of cases
Originally we estimated that an outbreak with over 1,000 cases should be detected. However, given the outbreaks in Italy, Iran and the US, we now have evidence that outbreaks can go undetected into the thousands of cases if the government is not looking. For example, [researchers have estimated 570 cases](https://hangouts.google.com/_/elUi/chat-redirect?dest=https%3A%2F%2Fbedford.io%2Fblog%2Fncov-cryptic-transmission%2F) originating from a single transmission chain in Washington. These were not detected by the CDC, but instead detected by independent researchers. So even in developed countries with good public health infrastrucuture, the government can miss transmission chains. India, for example, has only tested 3,404 individuals as of March 6th. In per capita terms, that's less testing that even the US, whose testing failures have been widely publicized.

As a result of low testing capacity, many countries have instituted testing protocols that only test travelers from China, South Korea, Iran, and Italy. For example, up until March 4th, [the US was only testing cases](https://web.archive.org/web/20200228190030/https://www.cdc.gov/coronavirus/2019-ncov/hcp/clinical-criteria.html?CDC_AA_refVal=https%3A%2F%2Fwww.cdc.gov%2Fcoronavirus%2F2019-ncov%2Fhcp%2Fidentify-assess-flowchart.html) with links to either an affected country or another confirmed case or the case is severe enough to require hospitalization. Since then, the official guidance has been for clinicians to use their judgement. This testing strategy would miss cases of community transmission or importations from countries that aren't covered by testing protocols.

However, the more time that passes, the less likely it is that cases can go undetected. For instance, if a given country has a thousand undetected cases, with a doubling time of about a week, there should be 16,000 cases a month later and 256,000 cases two months later. As time goes on, it becomes exponentially less likely that there are undetected transmission chains. If by April there are few detected cases then it's very unlikely these countries have outbreaks.

## Outbreaks outside of China are contained
One assumption of this forecast is that undetected cases can lead to large outbreaks that cannot be stopped once they’re detected. If instead these outbreaks are quickly stopped, that would be a signal countries are significantly better at responding to these outbreaks that we anticipated.

As of February 21, we are starting to see widespread outbreaks in Iran, and a worrying spike in cases in South Korea, possibly both caused by undetected lines of transmission. We’ll be watching to see how quickly these can be contained, if at all. If they are contained that leaves open the possibility of a middle ground scenario where we see new outbreaks regularly, but they are stopped quickly.

One cause for concern is that we expect there to be a high variance in how effective countries are at responding to an outbreak, and it may only require a few countries with a low ability to respond to spread the virus to the rest of the world.
