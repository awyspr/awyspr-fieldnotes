# 2026-04-07-here-comes-prm-again

## So whats this all about ?

While a lot of folk were getting into the chocolates over the Easter weekend, AWS have released new support info and capabilities for their previously released Partner Revenue Measurement (PRM) efforts. The [onboarding/getting started guide is updated](https://docs.aws.amazon.com/PRM/latest/aws-prm-onboarding-guide/getting-started.html)

There's basically 2 changes:

* Adding support for Metering
* Adding support for User Agents

### Metering

If you publish Amazon Machine Images (AMIs) or Machine Learning (ML) products to marketplace, then Metering is an important part of PRM for you - and prior to this release, you didn't get much love. 

But now its easy - [you don't have to do anything to make it work!!](https://docs.aws.amazon.com/PRM/latest/aws-prm-onboarding-guide/marketplace-metering-implementation.html) - essentially if you are publishing EC2 AMIs or Sagemaker AI ML models, you're already hooking the metering API when they are purchased and provisioned, and that data flows into PRM.

### User Agents

Perhaps the most notable addition is support for User Agent tagging of API/CLI calls as a partial alternative to Resource tagging. There's only a subset of services currently supporting the [PRM UA](https://docs.aws.amazon.com/PRM/latest/aws-prm-onboarding-guide/user-agent-included-services.html), so there's still a gap between Resource-taggable and User Agent-taggable services and the possible total set of AWS services that could make up a workload which is tracked for PRM purposes. 

The HOW-TO part is pretty easy if you have some AWS technical experience:

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
