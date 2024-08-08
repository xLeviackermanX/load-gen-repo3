# load-gen-repo
To use the Scale Test Load Gen App, users should maintain the same folder names but can choose any name and number of files within those folders. This structure will help keep the user's repository organised and make it easier to understand and navigate.



#### Folder Structure and File Content Type
```
load-gen-repo/            # Private github Repo Name
│
├── data-files/           # data-files, files used for API calls to Salesforce 
│   ├── accounts.csv       # in JMeter scripts.
│   ├── opportunities.csv
│   └── contacts.csv
│
├── test-plans/           # JMeter Script files
│   ├── use-case-1.jmx
│   ├── use-case-2.jmx
│   ├── use-case-3.jmx
│   └── use-case-4.jmx
│
├── user-files/           # or any other format storing usernames and passwords
│   ├── user1.csv
│   ├── user2.csv
│   └── user3.csv
│
├── workload-metadata/    # Metadata files describing orchestration tasks of tasks
    ├── b2b_workload_metadata.json       
    ├── b2c_workload_metadata.json
    └── integration_workload_metadata.json
```



---------------------------------------------------
|Folder Name	| File Content Type
----------------|---------------------------------
| **user-files**	| To store user credential files i.e. username and password which is used in jmx file.
| **test-plans**	| To store JMeter Script (.jmx) files.
| **data-files**	 | To be referred in the jmx files for various api calls to salesforce, sample repo has account.csv, opportunity.csv, contacts.csv but user can define file formats which they intend to use in their JMeter script files.
| **workload-metadata**	|To store metadata files which describes the overall orchestration by using the one script file for a task, all tasks would intiate workload execution in parallel.
---------------------------------------------------


### Note: 
This is only a sample repo.\
Users should keep this repo **private**.\
For a given workload, all the task names must be unique.\
Please avoid using any special characters for file names.
