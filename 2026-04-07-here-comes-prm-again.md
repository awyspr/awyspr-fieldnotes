# 2026-04-07-here-comes-prm-again

## So whats this all about ?

While a lot of folk were getting into the chocolates over the Easter weekend, AWS have released new support info and capabilities for their previously released Partner Revenue Measurement (PRM) efforts. The [onboarding/getting started guide is updated] (https://docs.aws.amazon.com/PRM/latest/aws-prm-onboarding-guide/getting-started.html)

There's basically 2 changes:

* Adding support for Metering
* Adding support for User Agents


missing cnp


``
  "eventName": "RunInstances",
  "eventSource": "ec2.amazonaws.com",
  "userAgent": "APN_1.1/pc_xxxxxxxxxx$ aws-cli/2.0.0",
  "sourceIPAddress": "203.0.113.12",
  "resources": [
    {
      "accountId": "123456789123",
      "type": "AWS::EC2::Instance"
    }
  ]
}``


### The Wrap Up

Still, the addition of User Agents helps close some gaps and provide some alternatives to the problems of using Resource tagging as we wrote about and experimented with earlier.
