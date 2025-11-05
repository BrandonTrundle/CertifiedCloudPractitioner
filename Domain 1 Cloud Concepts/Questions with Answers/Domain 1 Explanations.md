# 🧠 **Domain 1: Cloud Concepts — 30 Explanation-Based Questions**

---

### **Task 1.1 – Define the benefits of the AWS Cloud (value proposition)**

1. Explain in your own words what “economies of scale” mean in the AWS Cloud, and how AWS passes those savings to customers.
   Economies of scale refers to AWS' ability to pass cost savings to their customer, because of the vast amount of customer usage that AWS already has. In short, because AWS has so many customers it enables them to offer their services at a lower rate.

---

2. Describe how global infrastructure contributes to lower latency and better customer experience.
   The AWS global infrastructure contributes to lower latency and better customer experience by offering their services across a vast amount of regions. The have regions all over the world, with many including several different availability zones. AWS Edge Locations top this off, enabling AWS to cache content which in turn helps the customer deliver their resources to the customer no matter where they are.

---

3. Distinguish between **agility**, **elasticity**, and **scalability** — and give a real-world example of each.
   Agility is the ability of a company or individual to expirement with IT resources in the cloud, without having to invest in CapEx. Elasticity is the ability to automatically scale your resources to meet the demand of your workloads. Scalability goes hand in hand with elasticity. You can either scale horizontally or vertically, or both depending on your needs. Scaling horizontally is when you add extra resources to meet your demands, like adding extra EC2 servers. Vertical scaling refers to increasing the raw power of the resources you already have. For example, if the server you selected wasn't powerful enough to meet your demand, and you need to increase its size: t2.micro -> t3.large.  
   Real world examples:

- Agility: A startup company has almost fnished a brand new software project, and is considering deploying the software project to the cloud. Agility allows them to test the product with no upfront CapEx, and with little risk.
- Elasticity: The same startup company decided eventually to deploy to the cloud. They have selected a right size EC2 instance for their workload, and during peak hours scale their resources both automatically and horizontally. When business slows down, they decrease their deployed resources to meet demand automatically.
- Scalability: I touched on this with elasticity, but let's say that during the last peak season while the startup company's resources were deployed, they noticed high CPU usage on the deployed instances. They can easily scale vertically to fix this. On the other hand, if they had no high CPU usage, and just wanted to scale horizontally they can do that also.

---

4. How does moving from CapEx to OpEx change a company’s financial risk profile?
   When a company doesn't deploy to the cloud, and needs compute, it means that they have to invest in their own hardware, labor, building, and electrical costs. This directly relates to things like purchasing servers to host their resources, hiring people to build and manage those resources, they could potentially have to buy extra space to house those resources, and must make sure that the server room(s) remain at an appropriate temperature to keep the machines from overheating. Migrating to the cloud eliminates all of these expenditures. There's literally no reason to ever really want to invest that money unless required (compliance requirements - Hospital must have keep patient records on-premises for example)

---

5. Explain why **high availability** and **fault tolerance** are not the same thing, and how AWS designs for both.
   High availability and fault tolerance do go sort of hand in hand, and are often spoken of in the same breath. However, HA refers to architecture where resources have been deployed into multiple AZ's but one AZ is the "main" AZ, while the other is considered to be on "standby". Both would still use an ALB to transfer the customer to the working one, HA just allows for a little bit of down time in between. Fault tolerance on the other hand is architected for absolutely 0 down time. When you create architecture that is falt tolerant, it means that the deployed resources in the AZ's are BOTH active. Neither is on standby.

---

6. A startup wants to launch globally next week with minimal hardware investment — walk through exactly how AWS enables that.
   Well, I think this really depends on what the start up really needs. However, in order to global, AWS literally says the phrase "Go global in minutes". This has to do with the AWS Global infrastucture. You can deploy your IT reources to a region where your customers are located with the click of a button. Important here is: AWS Regions, AWS Availability Zones, AWS Edge Locations.

---

7. Why is **speed of experimentation** considered a core business benefit of cloud computing?
   The reason that speed of experimentation is considered core business benefit is because customers use pay as you go pricing to experiment with the AWS cloud, instead of having to purchase their own hardware to do the job.

---

8. Describe how **AWS’s global reach** benefits compliance and data sovereignty requirements.
   AWS has services like AWS Artifact that customers can use to make sure that they remain compliant. Need info on ISO27001 compliance? Go to AWS Artifact. HIPPA? AWS Artifact. Because AWS has customers all around the world, and have been operating for so long, they also have already laid the foundation for us to follow what they have discovered to be best practice when referring to things like data sovreignty and compliance. There are also a great deal of tools we can use after we understand what our requirements are, that will help us to make sure we remain compliant. How we encrypt data (both in transit and at rest) for example, or using trusted advisor.

---

### **Task 1.2 – Identify design principles of the AWS Cloud (Well-Architected Framework)**

9. In your own words, summarize the purpose of the AWS Well-Architected Framework.
10. Choose one pillar (other than Security) and explain how it reduces business risk.
11. How does the **Operational Excellence** pillar tie into continuous improvement cycles like DevOps?
12. What trade-offs might exist between **Cost Optimization** and **Reliability**, and how should architects balance them?
13. Explain how **automation** supports multiple pillars at once.
14. Pick an AWS service and map it to at least two Well-Architected pillars, explaining why.
15. How does the **Sustainability** pillar extend the concept of shared responsibility?
16. Why is _performance efficiency_ about more than just using larger instances?
17. If a workload consistently exceeds performance expectations but costs keep climbing, which pillars are in conflict and how would you adjust?
18. Describe what it means to perform a **Well-Architected Review**, and what outcomes it produces.

---

### **Task 1.3 – Understand the benefits of and strategies for migration to the AWS Cloud**

19. Explain the purpose of the **AWS Cloud Adoption Framework (CAF)** in a migration project.
20. A company wants to “lift and shift” 200 VMs, but later optimize them. Which migration strategies apply and why?
21. Describe the **6 R’s** in your own words, with one example for each.
22. Explain why migration is not only a technical change but also an **organizational transformation**.
23. How does using **AWS Snowball** differ from **AWS DataSync** during migration, and when would you choose one over the other?
24. What role does the **AWS Migration Hub** play in large-scale migrations?
25. Describe how **AWS CAF’s People and Governance perspectives** influence migration success.
26. How can the **AWS Cloud Adoption Framework** help a company measure business value post-migration?

---

### **Task 1.4 – Understand concepts of cloud economics**

27. Explain **variable costs vs. fixed costs** in cloud vs. on-prem environments.
28. What is **rightsizing**, and how does it differ from auto scaling?
29. How do **managed services** like RDS or DynamoDB contribute to better cost efficiency compared to self-managed equivalents?
30. Describe how automation (for example, through CloudFormation or Lambda scheduling) directly impacts cloud economics.

---
