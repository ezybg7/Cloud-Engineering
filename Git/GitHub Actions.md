Workflow is stored in yaml file
## Basics
Events
Jobs
Runners
Steps
Actions

```yaml
name: Super-Linter

#Event being monitored
on: push

#After event happens jobs is ran
jobs:
	super-lint:
		name: Lint code base
		#Job then runs on a ubuntu container hosted on git
		runs-on: ubuntu-latest 
		#steps
		steps:
			#first step is to checkout code
			- name: Checkout code
			  uses: actions/checkout@v2
			#then it runs this after checking out code
			- name: Run Super-Linter
			  uses: github/super-linter@v3
			  env:
				  DEFAULT_BRANCH: main
				  GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

