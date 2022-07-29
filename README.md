# Notes

This will clone our repository on the working directory
- actions/checkout@v1

To set a schedule we can use 
- https://crontab.guru/

To run a dispatch use

´´´
curl \
  -X POST \
  -H "Accept: application/vnd.github+json" \ 
  -H "Authorization: token <TOKEN>" \
  https://api.github.com/repos/salitomeyo-learning-path/udemy-github-actions/dispatches \
  -d '{"event_type":"build","client_payload":{"unit":false,"integration":true,"env":"production"}}'
´´´

We can use the following cheat sheet to create filter patterns
https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#filter-pattern-cheat-sheet
