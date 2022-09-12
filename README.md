# Module 9: Migration and Innovation

[AWS Cloud Practitioner Home](https://github.com/pslucas0212/AWS-Cloud-Practioner)

### Introduction

#### Transcript
So looks like we've established how to get going on the AWS Cloud, but what if you have existing deployments in on-premises environments or have started a cloud journey without AWS? Well, we'd love to help you move across, especially since you can take advantage of some real savings by moving. 

This brings us to migration and innovation. We'll show you all the options from migration tools, the AWS Cloud Adoption Framework, and even the Snow Family, which are physical devices to migrate data in and out of AWS. 

So before we adjourn, stay glued to your seats for information on how to move from on-premises environment or the cloud to AWS. We'll even cover the six Rs of migration.

### AWS Cloud Adoption Framework (AWS CAF)

Different team members bring different perspectives (finance, business, operations, development, etc.).

AWS consulting services has created the AWS Cloud Adoption Framework (AWS CAF) to assist with quick and easy migration to the cloud

AWS CAF Perspectives
- Business Capabilites
  - Business
  - People
  - Governance
- Technical capabilites
  - Platform
  - Security
  - Operations

Crate AWS CAF action plan.


#### Transcription
Migrating to the cloud is a process. You don't just snap your fingers and have everything magically hosted in AWS. It takes a lot of effort to get applications migrated to AWS, and having a successful cloud migration is something that requires expertise. 

Luckily, many people have had successful cloud migrations in the past, and you're not the first one to have solutions in AWS. Because of this, a lot of the knowledge around how to go about hosting on AWS has been captured and shared. 

That being said, what position you hold in your organization will impact the things that you need to know or help with for your migration. If you are a developer, your role and viewpoint will be much different than a cloud architect, business analyst or financial analyst. Different types of people bring different perspectives to the table for migration, and you want to harness those different perspectives and make sure everyone is on the same page. 

You also want to ensure that you have the right talent to help support your migration, so HR will need to hire at the correct rate to enable your migration. This can be a lot to keep track of, and someone new to the cloud might not think of all the different people who need to be involved. 

The AWS professional services team has created something called the AWS Cloud Adoption Framework that can help you manage this process through guidance. The Cloud Adoption Framework exists to provide advice to your company to enable a quick and smooth migration to AWS. 

The framework organizes guidance into six areas focused on the different types of people that you'll need to involve for your migration. Just like the different perspectives that we talked about earlier. Each Perspective covers distinct responsibilities covered by different groups. The different Perspectives are Business, People, and Governance Perspectives, which focus on the business capabilities, and then you have the Platform, Security and Operations Perspectives which focus on the technical capabilities. Someone who is a business or finance analysts would fall under the Business Perspective, HR would fall under the People Perspective, and a cloud architect would fall under the Platform Perspective.
 
Each Perspective is used to uncover gaps in your skills and processes, which are then recorded as inputs. These inputs are then used as the basis for creating what is called an AWS Cloud Adoption Framework Action Plan that you then use to guide your organization's change management as you journey to the cloud. Having an action plan that makes sense for your organization can help keep you on track. 

Migrating to the cloud can be complicated, but again, you're not alone in this, there are tons of resources to help you get started, and the Cloud Adoption Framework is a great place to look.


### Migration Strategies

Six Migration Strategies - Cost, time, priority, critical
- Rehosting - "lift and shift" "Move existing app/vm as-is to AWS. No optimization.  Save up to 30% by replatforming.  Easier to optimize once in the cloud.
- Replatforming - "Lift, tinker and shift".  Might make a few cloud optimization.  No new dev efforts.  Migrate from MySQL to Amazon RDBS
- Retire - app is no longer needed - AWS found 10 to 20% no longer are needed or already have been replaced.
- Retain - some apps will be deprecated soon.  You could migrate to AWS, but they will be turned off in 3 to 12 months.
- Repurchasing - Abandon legacy vendors to get a fresh start.  Or moving from license/sub model to software-as-a-service and PAYG
- Refactor/reachitecting - writing new code.  Highest initial cost and effort, but will benefit from cloud native services.


#### Transcript
So it is finally time to migrate from your on-premises deployment onto AWS. Like Morgan said in the prior video, it would be great to just snap your fingers and instantly have all the elements from your existing on-prem data center magically appear on AWS, optimized and efficient. But it doesn't work that way. 

Every application, or application groups, if they're tightly coupled, will have six possible options when it comes to your enterprise migration. We call these the six R's. Once you've gone through the discovery phase and know exactly what you have in your existing environment, you decide which option among the six R's is the best fit based on time, cost, priority, criticality. 

The first option is Rehosting. This is otherwise known as lift and shift. And this is an easy thing for businesses to do because you're not making any changes. At least not at first. Just pick up the applications and move them pretty much as is onto AWS. You may not get all the possible benefits. But some companies found that even without any optimization, they could save up to 30% of their total costs just by rehosting. Also, we find it's easier to optimize applications later once they already live in the cloud. Because your organization has better skills to do so. The hard part, the migration, is already complete. 

The second option is called Replatforming. Or lift, tinker, and shift. It's still basically a lift and shift, but instead of a pure one-to-one, you might make a few cloud optimizations. But you're not touching any core code in the process. No new dev efforts are involved here. For example, you could take your existing MySQL database and replatform it onto RDS MySQL, without any code changes at all. Or even consider upgrading to Amazon Aurora. This gives significant benefit to your DBA team as well as improved performance without any code changes. 

Now, before we add more migration options two of the six R's don't actually end up on AWS. Number three, Retire. Some parts of your enterprise IT portfolio are just no longer needed. We found as much as 10% to 20% of companies application portfolios include applications that are no longer being used or already have replacements live and functional. Using the AWS migration plan as the opportunity to actually end-of-life these applications can save significant cost and effort for your team. Sometimes you just have to turn off the lights. 

Number four, Retain. Some applications are about to be deprecated but maybe not just yet. They still need to run but don't turn them off for another three months or eight months. These apps could be migrated to AWS, but why? You should only migrate what makes sense for your business. And then as time goes on, these applications can be deprecated where they live, and ultimately retired. Okay, let's get back to what is going to move to AWS. 

Number five, Repurchase. This is common for companies looking to abandon legacy software vendors and get a fresh start as part of migration. For example, ending a contract with an old CRM vendor and moving to a brand new one. Or perhaps finally ending your licensing with an out of date database vendor in favor of cloud native database offerings. Now, this sounds great, but remember, you'll now be dealing with a new software package and some are easy to implement, some take time. The total upfront expense of the step therefore goes up, but the potential benefits could be substantial. 

Number six, Refactoring. Now, you're writing new code. This is driven by a strong business need to add features or performance that might not be possible on prem, but now are within your reach. Dramatic changes to your architecture can be very beneficial to your enterprise but this will come at the highest initial cost in terms of planning and human effort. 

Six paths to move to AWS. Once you have the inventory of all your pieces, choosing the right one for each part is critical to the success of your migration.

### AWS Snow

- AWS Snowcone - 8TB of data.  Place order on AWs console.  Plugin, copy data and send to AWS.  AWS copies to S3 bucket.
- AWS Snowball Edge - Compute optimized options or data optimized option.  Plugin to network and you can run simple processes on these devices
- AWS Snowmobile - Housed in 45 foot shipping container.  Houses 100 PB data - use for datacenter shutdown.  Plugin to network and copy data.

All devices designed to be secure and tamper resistant - all data is encrypted with 256-bit keys managed by the customer

#### Transcription
Some of our customers need to get data to AWS and most of them would like to do it in an efficient and timely manner. The usual route is to simply copy the required data over the internet or better yet, if they have a Direct Connect line. However, with the limitations of bandwidth, in general, this can take days, weeks, or even months. 

For example, a dedicated one gigabyte per second network connection theoretically moves one petabyte of data in about 100 days and in the real world likely longer and at a higher cost, with this customer feedback and as a way to address this gap, we therefore introduce AWS Snow Family of devices. 

The first device, which is also our newest offering, is called AWS Snowcone and it's a device that holds up to eight terabytes of data and contains edge computing. Edge computing options are Amazon EC2 instances and AWS IoT Greengrass. To obtain one, you place an order via AWS Management Console we ship it to you, you plug it in and copy your data, and finally, ship it back to us. We'll then copy the data to your AWS account, usually an Amazon S3 bucket that you own, and boom, Bob is your uncle and your data is available to use. Customers usually use these devices to ship terabytes of information such as analytics data, video libraries, image collections, backups, and even tape replacement data. I mean, who doesn't have a terabyte collection of cat images, that they want to backup to the AWS Cloud? 

But what if eight terabytes is not enough? Well, good news, we have a product for that requirement called Snowball Edge. It comes in two versions: a Snowball Edge Compute Optimized option and a Snowball Edge Storage Optimized option. Even better is that they fit into existing server racks and can be clustered for greater computing needs. Ones you plug them into your infrastructure, you can even run AWS Lambda functions, Amazon EC2-compatible AMI's, or even AWS IoT Greengrass to perform simple processing of data right then and there. Customers usually ship these to remote locations, where it's trickier to have a lot of computing power lying around. The use cases include capturing of streams from IoT devices, image compression, video transcoding, and even industrial signaling. 

The last device that's up for grabs is also the largest in our fleet, the AWS Snowmobile, and as the name suggests, it's housed in a 45-foot rugged shipping container and pulled along by a freaking truck, I mean this thing is huge. It houses 100 petabytes and is ideal for the largest migrations and even data center shutdowns. We drive the truck to your designated location, plug it in, and it then appears as a network attached storage device with, like I said, capacity of up to 100 petabytes. It is tamper resistant, waterproof, temperature controlled, it even has fire suppression and GPS tracking. I mean, can you believe that it also has 24/7 video surveillance with a dedicated security team and escort security vehicle during transit? That's some serious business. 

But it should be noted that all Snow Family devices are designed to be secure and tamper-resistant while on-site or in transit. This means the hardware and software is cryptographically signed, and all data stored is automatically encrypted using 256-bit encryption keys, owned and managed by you, the customer. You can even use AWS Key Management Service to generate and manage keys. 

As always, it's been a pleasure taking you through yet another AWS service. Hope you've had fun learning about the AWS Snow Family.

### Innovation with AWS

So much more... Like VMware on AWS - VMWare on cloud
ML and AI - broadest ML and AI services.  Pre-trained resources
Sagemaker - quickly build ML models
Amaazon Augmented AI (Amazon AI2)
Amazon Lex - heart of Amazon Alexa
Amazon Textract
AWS Deepracer - ML learning experience for developers
Internet of Things
AWS Ground Station - support for satellite usage


#### Transcript
There's so much more that can be done on AWS that we have time to talk about here. For example, when it comes to migrating onto AWS, we didn't even cover running VMware on AWS. The same VMware based infrastructure that you use on prem can in many cases, just be lifted up and dropped onto AWS via VMware Cloud on AWS. And this is just one of many concepts that make AWS a place where builders go to create and innovate at the pace of their ideas. 

When it comes to machine learning and artificial intelligence, AWS has the broadest and deepest set of machine learning and AI services for your business. You can choose from pre-trained AI services for computer vision, language recommendations, and forecasting. Amazon SageMaker: Quickly build, train, and deploy machine learning models at scale. 

Or build custom models with support for all the popular open-source frameworks. Our capabilities are built on the most comprehensive cloud platform, optimized for machine learning with high performance compute and no compromises on security and analytics. Tools like Amazon SageMaker and Amazon Augmented AI, or Amazon A2I, provide a machine learning platform that any business can build upon without needing PhD level expertise in-house. Or perhaps, ready-to-go AI solutions like Amazon Lex, the heart of Alexa.

[Alexa] Hello . What can I help you with?

Helps you build interactive chat bots.

Or what about Amazon Textract. Extracting text and data from documents to make them more usable for your enterprise instead of them just being locked away in a repository. 

Do you wanna put machine learning literally into the hands of your developers? Why not try AWS DeepRacer? A chance for your developers to experiment with reinforcement learning. One of the newest branches of machine learning algorithms, all while having fun in a racing environment. 

AWS offers brand new technologies in things like Internet of Things. Enabling connected devices to communicate all around the world. 

Speaking of communication around the world, have you ever wanted to have your own satellite? Too expensive to launch your own? Why not just use AWS Ground Station and only pay for the satellite time you actually need? 

I could go on for days talking about all these new technologies. Like literally for days. AWS Training and Certification offers training classes on many of these technologies already, and every month, AWS seems to release something even better for us to talk about.

### Summary

AWS CAF
Six Rs of migration - rehost, replatform, repurchase, retire, retain, refactor
Snowball - data transfer avoding the internet

#### Transcript
Over the last few videos, you started to learn about migration to AWS, as well as some interesting and innovative services you can use to either aid in your migration or to step your game up with AWS. 

You learned about the AWS Cloud Adoption Framework. The Cloud Adoption Framework gives you guidance on who to loop into a cloud migration, what their roles are, and the sorts of things that they should be focused on. There's the Business, People, and Governance Perspectives for nontechnical planning, and the Platform, Security, and Operations Perspectives for technical planning. 

We also talked about the six R's of migration. The R's represent different strategies on moving solutions to the cloud. They are Rehost, Replatform, Repurchase, Refactor, Retire, and Retain. 
There was also the question of how to move massive amounts of data into AWS without going over the network. This is where you learned about AWS Snowball and AWS Snowmobile, which allow you to fill in a physical device with your data and have it shipped back to AWS who then uploads it for you. This is useful to sidestep any potential throughput issues, and it is also more secure than using high-speed internet.
