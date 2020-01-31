# The Hitchhiker's Guide to AI & ML in AWS workshop
### Exploring AWS Rekognition

## STEPS

    IMAGE=example.jpg

    aws rekognition detect-labels --image-bytes fileb://$IMAGE --output json | jq .

    aws rekognition detect-text --image-bytes fileb://$IMAGE --output json | jq .

    aws rekognition recognize-celebrities --image-bytes fileb://$IMAGE --output json | jq .

    aws rekognition detect-moderation-labels --image-bytes fileb://$IMAGE --output json | jq .
