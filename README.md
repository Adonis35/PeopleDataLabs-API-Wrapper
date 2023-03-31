# People Data Labs API Wrapper

### Authors: Adonis Abdullah
Developed an API wrapper for my former employer, <a href="https://www.oldwellpartners.com/">Old Well Partners</a>, to allow engineers and data scientists to easily access and utilize <a href="https://www.peopledatalabs.com/">People Data Labs'</a> API. This wrapper would return data on companies' employees and individuals' employment history in json format that could then be implemented into different projects. 

```python
from pdlabs import PDLAPI

SAMPLE_QUERY = """
  SELECT * FROM person
  WHERE location_country='mexico'
  AND job_title_role='health'
  AND phone_numbers IS NOT NULL;
  """

pdl_api = PDLAPI()

# send a query to the person search API:
# https://docs.peopledatalabs.com/docs/search-api
response = pdl_api.search_person_api(query=SAMPLE_QUERY)

print(response)
```


#### Responsibilites:
* Developed API Wrapper

#### Technologies:
* Python

#### Outcomes:
* Deployed wrapper internally
* Implemented in company's internal investment site
* Implemented in company's commercial investment site

#### Technology Owner:
* Old Well Partners
