# PlantUML Github Workflow
When Puml files are pushed to repo, Github Actions generate png and svg diagrams in diagrams dir, and commit these to repo.

For overview, see https://www.mytechiebits.com/GithubActionsWorkflow

See .github/workflows/main.yml for the workflow file.

From our local repo, we want to be able to push without having to pull the diagrams newly created by the workflow.
One way to achieve this is to add the in diagrams/ dir to .gitignore.
But then we need to add "-f" option to force the workflow script to add the files (that are in the .gitignore)

````
          git add -f --all ${{ env.OUTPUT_DIR }}/*
````