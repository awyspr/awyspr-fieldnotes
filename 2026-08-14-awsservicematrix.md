<a href="https://awyspr.com/"><img src="https://awyspr.com/assets/images/image07.svg?v=b4a015c2" width="10%" height="10%" align="left"></a>

# Which AWS services are available in which region ?

2026-08-14

## What's this one all about then ?

Which AWS services are live in which regions ? This might seem like a fairly simple question, but its important if you're 
deploying something and you want it to be regionally-contained, eg for digital sovereignty reasons or because of end user 
proximity and performance.

There are some AWS services which are "in every region", and others are far less widely available. Want Bedrock ? Pick 
any default or opt-in region except ap-east-1 (Hong Kong). Want Macie ? Your choices are more limited, particularly if 
you are in APJ. What's the difference in the range of services available in ap-southeast-2 (Sydney) and ap-southeast-4 (Melbourne) 
? Or between eu-central-1 (Frankfurt) and eu-central-2 (Zurich) ?

awyspr 's unofficial AWS Service Matrix builds a view from AWS' own public inventories and data feeds to show which services 
are available where, with daily automated updates, and without needing to mess about in the AWS console or with the CLI. 

Take a look, and you might be suprised: [https://awsservicematrix.info](https://awsservicematrix.info/)

## The wrap up

In the world of AWS, not all services are created equal, and not all regions are either. That's not a criticism, its reality, and hopefully
our tool https://awsservicematrix.info helps people understand the diversity a bit more.

[Back to awyspr fieldnotes index](https://fieldnotes.awyspr.com)
