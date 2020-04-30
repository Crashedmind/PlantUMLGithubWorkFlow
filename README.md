# PlantUML Github Workflow
When Puml files are pushed to repo, Github Actions generate png and svg diagrams in diagrams dir, and commit these to repo.

For overview, see https://www.mytechiebits.com/GithubActionsWorkflow

See .github/workflows/main.yml for the workflow file.

# Usage

1. Copy the  .github/workflows/main.yml workflow file to your repo
2. Push changes to github
3. Add some PlantUML *.puml files
4. Push changes to github
5. Diagrams should be auto generated in diagrams/
6. 