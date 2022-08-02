# Chapter 1. Analyzing Business Domains
[Read Chapter 1 on O'Reilly](https://learning.oreilly.com/library/view/learning-domain-driven-design/9781098100124/ch01.html#analyzing_business_domains)

What is the main point of this chapter
Why this chapter is important
What are the key take-aways of this chapter

---
## Business Domains and Subdomains:
**Business Domain** - A company's main area of activity.  The service or product the comapny provides to its clients.   
*note - a company can operate in multiple business domains*

**Subdomain** - A fine-grained area of business activity that does not contribute to the profitability of the company but is necessary for the business to operate.  There are 3 types of subdomains:  Core, Generic and Supporting.   
*It is not uncommon for subdomains to change types over time.  A core subdomain may become a generic subdomain as technology advances. Conversly, a generic subdomain my evolve over time and become a core subdomain*

**Core Subdomain (aka Core Domain)**  - Business Activities that support the business and are a source of competitive advantage.  This is something a company does differently from its competitors,  is hard for a competitor to copy or imitate the company's solution and therefore has complexity and high volatility to keep ahead of the competition.  Due to the competitive advantage the core subdomain provides
*Example:  Google Search - this is not a paid service but the search engine is an important component of the Google Ads product*

**Generic Subdomain** - Business Activites that support the business, is generic (all companies are performing in the same way) and does not provide any competitive advantage.  The solution is complex but not volatile (does not change often).  
*Example: An online retail platform used by many companies*

**Supporting Subdomains** - Business Activites that support the business, are not generic but also do not provide any competitive advantage.
*Example: Indexing a catalog of the compay's creative materials for use with Google Ads*

### Solution Strategy
**Subdomain Type** | **Competitive Advantage** | **Complexity** | **Volatility** | **Implementation** | **Problem** |
|--------------------|---------------------------|----------------|----------------|--------------------|-------------|
| Core               | Yes                       | High           | High           | In-house           | Interesting |
| Generic            | No                        | High           | Low            | Buy/adopt          | Solved      |
| Supporting         | No                        | Low            | Low            | In-house /outsource | Obvious     |

Identify the subdomains and their boundries to make good business decisions on how to solve these problems.  To buy a third-party solution or develop the solution in house for example.  
The subdomains and their types are defined by the company's business strategy.  To identify and categorize the subdomains of a company, see what the company departments are as well as other organizational units.  These are course-grained areas of activity.  
Distilling subdomains will uncover details we may not have seen at the department level.  For instance, we may not have thought that the Human Resources department not only needed HR related software, but also a help desk system for employees.  Drill down into the lower levels of granularity until further research does not unveil any new insights.
In this example, distilling the generic help desk system does not show us any non-generic inner subdomains.  We can determine that an off the shelf solution will be sufficient.  
![[Pasted image 20220802155333.png]]

*Note that an important consideration is, when identifying the inner subdomains, whether we need all of them, or can the same solution be utilized by other generic subdomains.  Does another department require a help desk system as well?  if so, can they use the same platform?*

