# The Hitchhiker's Guide to AI & ML in AWS workshop
### Exploring AWS Comprehend

## STEPS

    TEXT="Welcome to the Hitchhiker's Guide to AI & ML in AWS workshop"

    aws comprehend detect-sentiment --language-code en --text "$TEXT" --output json | jq .

    aws comprehend detect-entities --language-code en --text "$TEXT" --output json | jq  .
