# Template description

This repository contains the starter materials for your thesis in Computer
Science 600 and 610 in Fall 2022  and Spring 2023 academic term. The main
directory of this repository contains the Markdown template for a project that
is designed for use with GitHub Classroom. To learn more about the course
in which these assignments were completed, please refer to the `README.md` file.

The template specifies various settings in the `config.yaml` file included in the
repository. Change the appropriate values under the `Project-specific values`
heading. Changing other values outside of that section may cause the project to
fail to build. **Modify these values at your own risk.**

Author your thesis in the `thesis.md` document using appropriate Markdown
hierarchy and syntax; GitHub Actions will automatically create a PDF from the
`abstract.md` and `proposal.md` files. Consult the `README` of the proposal
repository to learn how to properly build and release this PDFs.

## Citations and references

Including references throughout requires a specific pseudo-Markdown tag, demonstrated
in the following blockquote. (Inspect the `thesis.md` file to see the format.)

> A citation, when included correctly, will appear as it does at the end of this
> sentence. [@plaat1996research]

## Labeling figures

To label a figure (i.e. an image), referencing the image using correct Markdown
will automatically caption the figure:

```markdown
![Label](images/IMAGE_NAME.png)
```

## Labeling tables

To provide a label for a table, write a short caption for the table and prefix the caption
with `Table:` as in the example below:

```
Table: A two-row table demonstrating tables

|Row number | Description |
|:----------|:------------|
|1          |Row 1        |
|2          |Row 2        |
```

## Other template information

Two things specific to this template to also keep in mind:

1. It is your responsibility to remove this description section before building
the PDF version you plan to defend.
2. References _will only appear if cited correctly_ in the text

## Note on `LaTeX` commands

Documents may include specific `LaTeX` commands _in Markdown_. To render these, surround the commands
with markup denoting `LaTeX`. For example:

```
Checkmark character:   $\checkmark$
Superscript character: $^{\dag}$
```

If using a special package not included in the template, add the desired `LaTeX`
package or command/macro to the `header-includes` property in [config.yaml](config.yaml).

Should this package not be included in the environment shipped with this template,
you may also need to add the package to the [GitHub Actions Workflow](.github/workflows/main.yml).

Direct any questions about issues to your first reader.

# Introduction

This chapter describes your completed senior thesis work,
including the overall aims  and the background motivating your research. Whenever
possible, you should use one or more concrete examples and technical diagrams.

It is often useful and necessary to separate the introduction into multiple sections.
Several possible sections are proposed below, you can use these or distribute your
introductory text into sections in another wayyy.

The headings below propose _one way_ you might structure this section of the document.

## Motivation

The US Census Bureau defines educational attainment as the highest level of education that an individual completes. Studying educational attainment is important because the level of education a person attains is oftentimes directly linked to the professional, personal, financial, and social opportunities available to a person. For example, a person with a lower level of educational attainment may not have access to job opportunities that require a high level of education. Or in contrast, a person with a high level of education may have access to opportunities and resources resulting from a higher social or financial status.

The level of educational attainment a person achieves could be impacted by differences in various demographic factors such as race, gender, and level of income. These demographic factors may have a say in how an individual’s personal expectations, limitations to access, and accessibility to informational resources informs their decision to pursue greater educational opportunities, such as a postsecondary education. The main goal of this research is to determine to what degree, if at all, these demographic factors (race, income, sex) play a role in determining an individual’s level of educational attainment.

There is evidence in how income, and more specifically socioeconomic status, can impact one’s education. For example, children from families with a low socioeconomic status “are less likely to have experiences that encourage the development of fundamental skills of reading acquisition” and “to have access to informational resources about college”. (APA) Not only are access to education and development of certain skills impacted by socioeconomic status, but so is academic achievement; low-income children “enter high school with average literacy skills five years behind those of high-income students”, have a lower success rate in the fields of “science, technology, engineering, and mathematics” than those not from underrepresented groups, and have a higher likelihood of dropping out of high school (11.6%) compared to their high-income counterparts (2.8%). (APA)

Additionally, research has shown that differences in educational attainment by gender have varied greatly over the last century, initially the trends appeared to be favorable to men but by 1982, women started to lead in rates of enrollment and graduation from high school and college. These gendered differences in educational attainment have various causes including gender expectations towards receiving a higher education, accessibility to education, opportunities available post-graduation, and personal aspirations in completing some form of postsecondary education. The gender disparities in educational attainment also intermingle with racial disparities as there are different historical trends between each racial/ethnic group and the dispersion of educational attainment also plays out differently for each group.

Race also has played a role in determining the level of education a person would complete for the better half of the last century. This is as a result of the type of opportunities to access education and ease of accessing this and other related resources available to these groups. Historical events and trends have also exacerbated the racial disparities in educational attainment such as the lingering effects of slavery and segregation.

1. explain why educational attainment study is important!
2. intro factors that can impact educational attainment study
3. explain why income is an important factor to study
4. explain why race is an important factor to study
5. explain why sex is an important factor to study

## Current State of the Art

1. explain that other projects dont usually look at intersection btwn these 3 factors
2. explain projects haven't looked at race differences outside black and white
3. explain projects recently haven't looked at income differences
4. few project employ a regression model to test for statistical significance of relationship

There has been a good amount of research done on the topic of educational attainment that has been able to capture differences in gender, race, and income, and their implications. The main focus in a lot of literature is on gendered differences in educational attainment, which seems to be a well-documented issue overall. These gendered differences seem to show that while there was at some point in time (in the past) a male-leaning dominance in levels of educational attainment, women seem to now hold the advantage in educational attainment. However, this gender gap reversal in educational attainment does not seem to reflect a reversal in the gender gap as it relates to occupations or wages.

When racial differences in educational attainment are studied, many authors tend to focus on the differences exclusively between white and black people. This neglects the disparities and differences in educational attainment that could be potentiall observed in other racial or ethnic groups. One of the goals of this study and subsequent tool is to analyze differences across different racial and ethnic groups, with special interest in observing differences in racial groups that literature has failed to cover.

In contrast, there seems to be a good breadth of literature studying the effects of income on educational attainment. This literature, however, is mostly outdated and does not touch upon if there have been any movements in trends of educational attainment. Another goal of this project is to expand on the research that has already been done on the effects of income, with special priority in seeing how this impact has changed and if there are any other different implications that have not yet been covered in the literature.

To date, there has not been research that looks at the combined impact of race, income, and gender on educational attainment and as there are various factors that can go into play in impacting whether or not a person will recieve a certain level of educational attainment, doing this research is important. It is not clear why these three factors haven't been studied in tandem before, but it can be presumed that it may be a result of complexities in researching the combined effects of these factors on attainment. Another goal of this project is to address this specific gap in measuring the combined effects in the literature.

Few studies employ the use of a regression model in order to study the effects of different factors on educational attainment, and the ones that are most likely to were on the topic of income. One of the goals of this project is to construct and run a regression model that includes the factors of race, income, and gender as they relate to educational attainment, and also regressions that look at each of these factors in isolation. This is in order to get the statistical significance of the relationships between each of these factors in relation to educational attainment, which can then be used to determine the strength of the relationship between each of the factors. It could also help determine which of these factors plays a bigger role as a determinant of educational attainment.

This project also looks to take on the task of an interdisciplinary study, as research from various fields of study including Sociology and Economics will be leveraged in the creation of a tool that is created using computer science and data science fundamentals. The goal is that this project represents a type of study called fusion analysis, where multiple disciplines are used together in order to analyze data and draw greater conclusions from that data (had only traditional data analysis been employed).

## Goals of the Project

1. brief project description + data description
2. brief implementation description
3. final product description

This project looks to study the impact of race, gender, and income on educational attainment in the United States. This project will use data from Integrated Public Use Microdata (IPUMS) Current Population Survey (CPS) microdata, which is harmonized and includes relevant demographic information. The data itself is cross-sectional, encompassing years 2010-2015 in the United States. Specifically, the variables in the data extract, created using IPUMS’ platform, include the survey year (YEAR), state identified by FIPS code (STATE), age (AGE), sex (SEX), race (RACE), Hispanic origin (HISPAN), educational attainment code (EDUC), total family income (FTOTVAL), and total personal income (INCTOT). Additional variables were included in the extract, for the purposes of aiding in identification of individuals and individual households, and analysis of specific data: household record of CPSID (CPSID), month (MONTH), household serial number (SERIAL), person number in sample unit (PERNUM), final person-level weight for analysis (WTFINL), and the person-level used for supplement data (ASECWT).

In order to access to all of the data, an SQLite database will be used to store the data to be used in RStudio to wrangle and transform data as needed in order to generate statistics and visualizations, telling of the trends present in different identity groups. These statistics and visualizations will then be output on a web platform that allows for a user to compare two different identity groups or to look at the trend of educational attainment for one identity group over the years.

The main goal of this project is to provide a tool that will make it easy to observe trends in educational attainment across different states and determining, within each of those states, the different race, gender, and income backgrounds accounted for and their levels of educational attainment within the sample. An auxiliary goal of this project is to be able to compare trends in educational attainment based on state, as well as, when grouped off by factor like gender, race, or income. This is so that the trends based on individual factors can be studied/observed in isolation, as well. A final goal of this project is to determine if there is a statistical relationship between educational attainment and each of these factors, and whether or not these factors can be viewed as determinants of educational attainment.

## Ethical Implications

This document requires that you discuss the ethical implications of your work -- no
matter how benign you consider the outcome of your project. As several major studies
of ethical issues in computer science assert: _no project is completely value-neutral_.

To assist you in elaborating on these issues, the following areas are topics you might
consider addressing. You do not need to address all of them.

* Information Privacy
* Information Accuracy (e.g. can contain reliability)
* Potential Misuse (e.g. computer crime, unintended consequences)
* Second- or Third-Party Risk (e.g. safety)
* Data Collection Issues (e.g. issues inherent in collecting data)
* Algorithmic or Data Bias
* Potential Power Difference / Social Imbalance / Issues in Equity

In addition, reflect on ways that the above harms can be or are mitigated by your work

There are a few ethical issues that need to be addressed within this work involving the security and reliability of the data used to analyze the trends of educational attainment across different groups. Additionally, there may be issues related to data collection, as the data only represents attainable and usable samples, as well, as, issues that may arise from the sourcing of the data. The source of the data, Integrated Public Use Microdata (IPUMS), harmonizes Current Population Survey (CPS) microdata to include relevant demographic information about individual people and households.

To address the first issue of reliability, the data itself is collected from a survey, meaning that responses are self-reported. This can be an issue if there is no general mechanism, within the Census' collecting of the data, that verifies the answers given to the survey. This could mean that certain answers could have been given in order to seem better than actuality. In the case of this study, there could have been someone who lied about their highest level of educational attainment or about their level of income in order to seem more or less well-off. Also on the note of survey data, there may also be issues in data collection that may be present. Things like incomplete surveys or filling out of data extracts (on IPUMS' behalf), may result in untrustworthy or inclusive statistics or results.

Additionally, there seems to be a potential issue in data collection or extraction, as there was a discrepancy between the data extract created for this project using IPUMS' extract tool and the actual data that ended up being usable for the project. The original intent of this project was to study data from the last 10 years in order to capture how educational attainment has changed over time, with help from the literature. But upon opening and working with the IPUMS data extract, which should have included years 2010-2021, it became clear that only data from 2010-2015 was accessible and usable. It is not clear if this is an issue resulting in incomplete data or with the data extract tool, but either way this could still be an issue future researchers may encounter with this tool.

As the data for this project was extracted and downloaded from a third-party tool, IPUMS' online data extract creator, there may be risks with using a service like this. Like mentioned above, there may be discrepancies with the data in that more data is expected in an extract than is actually given. There could also be issues in the accessibility of using this data, as an account is required to access the data. Additionally, there is the risk of just having to trust the reliability of the data provided by the third-party source.

In the initial use of the data, it became apparent that there may also be some data bias within the dataset. This is because when observations are counted by state, a varying amount of individuals are represented in each state, but never fully representing the populations actually present in those states. These counts also vary year to year, which further brings into question the validity of the data. The fact that this data only represents samples may bring up issues in the reliability of the data, in that it is unclear if there was any bias in the collection of the data or if the data may be incorrectly skewed towards representing one group over another.

The last but probably the most important ethical issue that may arise as a result of this project includes the potential issues in equity, that the project generally looks to address. Because this project is rooted in looking for trends in educational attainment, focusing in on gendered, racial, and financial disparities in attainment, the results of this project may have real implications for the groups represented. With that, there should be a great deal of consideration taken when looking at and comparing trends across groups, as well as, when introducing and talking about educational trajectories. This is in order to avoid an unneccessary harm or unreliable characterizations or representations of certain identity groups or specific regions.

# Related work

This chapter includes a broad and detailed review of relevant existing work.
The literature review should provide background and context for the thesis work.
The subsections may be organized in whatever manner seems best suited to the material--
chronological, or by topic, or according to some other criteria
(e.g., primary versus secondary resources).

If ethical issues are central to this work, you should also address historical and
contemporary issues or efforts made to address them.

# Method of approach

This chapter answers the "how" question - how did you complete your project,
including the overall design of your study, details of the algorithms and tools you
have used, etc.  Use technical diagrams, equations, algorithms, and paragraphs of text
to describe the research that you have completed. Be sure to number all figures and
tables and to explicitly refer to them in your text.

This should contain:

* lists
* with points
* and more points
  * possibly subpoints

For those projects whose implications address social or moral issues (i.e. ethical
standards, causes, effects), you will want to use this section to describe how you
actively mitigated or considered these issues.

# Experiments

This chapter describes your experimental set up and evaluation. It should also
produce and describe the results of your study. The section titles below offer
a typical structure used for this chapter.

## Experimental Design

Especially as it pertains to responisble computing, if conducting experiments or
evaluations that involve particular ethical considerations, detail those issues here.

## Evaluation

## Threats to Validity

# Conclusion

Traditionally, this chapter addresses the areas proposed below as sections, although
not necessarily in this order or organized as offered. However, the last section --
"Ethical Implcations" is required for this chapter. See the heading below for more
details.

## Summary of Results

## Future Work

## Future Ethical Implications and Recommendations

Especially as pertains to the public release or use of your software or methods, what
unresolved or special issues remain? What recommendations might you make?

## Conclusions


# References

::: {#refs}
:::
