# Deploy an E-commerce Site (Magento) on AWS App Runner

## Deployment Instructions

1. Open the [CloudFormation template for a dev environment (dev-env.json.zip)](/dev-env.json.zip) in a new browser tab (ctrl + click OR command + click).
1. Download and extract it. It will be used later.
1. Sign-in to your [AWS console](https://console.aws.amazon.com/).
1. Transfer to Tokyo region.
1. Go to [CloudFormation](https://ap-northeast-1.console.aws.amazon.com/cloudformation/home?region=ap-northeast-1).
1. Deploy dev-env.json in CloudFormation.
1. Wait for the creation to complete.
1. Sign in to Magento Marketplace.
1. Create Magento access keys. Keep the window open. You'll need the values later.
1. Open C9forSS environment in Cloud9.
1. Run the following commands from the terminal:
```
git clone https://github.com/engr-lynx/aws-mage-be.git
cd aws-mage-be
. ./bin/env.sh
./bin/deploy.sh
```
1. Visit App Runner after 30 mins to get the link to your e-commerce site.
1. Important: Don't forget to clean-up your deployment after the designated time. Unless... you intend to keep on using and building on top of it.

### Clean-up Instructions

1.
