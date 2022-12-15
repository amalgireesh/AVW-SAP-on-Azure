Azure Virtual Workshop: SAP on Azure

## Overview

SAP on Azure solution helps you optimize your Enterprise Resource Planning (ERP) in the cloud using the security features, reliability, and scalable SAP-certified infrastructure of Azure.

When managing a global, distributed supply chain and manufacturing environment, companies face challenges with constrained bandwidth, latency issues, and massive volumes of data that can adversely influence execution and quality scenarios.

SAP uses Microsoft Azure to run these solutions in a software-as-a-service (SaaS) model that can help reduce the customer’s need to manage the software and underlying infrastructure while accelerating the time to value of supply chain applications. Customers will be able to scale globally by leveraging Azure which offers enterprise-grade compute, storage, and network services to support mission-critical performance and business continuity to run SAP Digital Supply Chain solutions.


## Hands-on Labs Scenario

For the lab, let’s consider Contoso which is a large company that handles logistics. Currently, to keep up with the global crisis with the supply of vaccinations, Contoso is responsible for shipping vaccines across the world. Such a massive scale of logistics is often challenged by various factors, one of which is the time constraints and maintaining the correct temperature (30 degrees) of the storage containers, exciding that will result in wastage of the vaccine.

Hence, one of the core functions of Contoso's vaccine supply chain is to maintain the temperature threshold of the vaccine containers and stabilize the temperature at every step of the entire transition. They are required to maintain the proper temperature for products that cannot tolerate excessive heat, especially in places with an extremely hot climate, unreliable connections to electricity, or poor transportation infrastructure. Temperature monitoring is a critical thing for Contoso to assess vaccine handling quality, detect malfunctioning equipment, and understand if it has negatively impacted vaccine potency and safety.

To tackle this, Contoso has included IoT devices with temperature sensors in each package. Contoso allows you to connect to those devices in an Azure IoT Solution and retrieve the temperature readings from the package which will be then used to monitor or to place a replacement order for any vaccine that gets damaged.

## Lab Context

Contoso wants to make sure that the vaccine is not exposed to unstable temperatures as that will result in irreversible damage to the vaccines. So, Contoso requires a way to monitor the temperature data generated by the built-in sensors and evaluate if the vaccine needs to be replaced in case the temperature goes above 30°. Contoso wants an order to be placed automatically to replace the damaged vaccine in case the measured temperature goes above 30°. 

Contoso also wants to integrate the SAP system and Microsoft Azure to view the Sales Order data in a Teams channel or through an e-mail in Outlook. Contoso uses SAP Systems to store information related to the products they provide. Currently, the process to add a new product into the catalog is by first sending the Product Information to the Manager over email for approval. Once approved, the product details are entered manually into the catalog via the SAP Fiori Web Application. Contoso now wants to eliminate the manual procedure and transform their manual business processes to digital, automated processes using Power Apps, Power Automate.

Contoso hosted large-scale workloads with SAP on Azure, and wants to address security, governance, performance, and cost concerns of deployments in one or more regions throughout the lifecycle of cloud services. It wants to leverage governance, which is an ongoing process of managing, monitoring and auditing the use of Azure resources in order to meet the organization's goals and requirements. Contoso also wants to apply specific security controls to the operating system, data, and SAP application using Azure Security Center.

This lab includes the following modules. 

## Module 2 - DataInsights

This module covers how to use Power BI, Analytics, AI, and IoT to extend and innovate data insights with SAP on Azure.

In this module, you will review the pre-deployed resources, connect to the Azure IoT Hub device and send telemetry data from the device to Azure IoT Hub. You will then configure a route in the Azure IoT Hub to direct the messages to the service bus queue as soon as the temperature reaches 30°C/86°F or more. Then you will configure a Logic App to be triggered by a Service Bus queue which will send an e-mail notification to you whenever a message is added to the queue and automatically creates a sales order in the SAP system.

You will also enable viewing the current sales orders in Excel, PowerBI, Outlook, and Teams.

Below is the diagram of the **Solution architecture** that you will implement in this lab.

![](https://github.com/CloudLabsAI-Azure/AIW-SAP-on-Azure/blob/main/media/M2-Ex4-architecture.png?raw=true)

## Module 2 - Productivity

This module covers how to use SAP on Azure to improve productivity and collaboration in your workplace.

In this module, you will configure a Logic App to display the SAP ERP data in Teams and send an email of the latest sales order data to Outlook at regular intervals.

Below is the diagram of the **Solution architecture** that you will implement in this module.

![](https://github.com/CloudLabsAI-Azure/AIW-SAP-on-Azure/blob/main/media/M2-Ex6-architecture.png?raw=true)

## Module 3 - App Innovation

The SAP platform provides a foundation for innovation for many companies and can handle various workloads natively. This module covers how to innovate using Artificial Intelligence, Machine Learning, and Power Apps with SAP running on Azure.

In this module, you will create a custom connector and Power App then add the custom connector to the app, which will be used to connect to your SAP System. Then, you will create and train the AI model to process the information from documents using AI Builder. You will also configure a workflow to process information from the documents by using an AI model, send the Product Information to the Manager over email for approval and add products to the catalog once the request is approved by the Manager. You will then trigger the workflow and verify the products that are added to the catalog by the workflow.

## Module 3 - Cloud Operations, Governance, Security

This module covers how to operate and govern the SAP system running on Azure.

In this module, you will review the pre-deployed SAP HANA resources, connect to the SAP HANA database and verify the status of the database. You will also review the CPU and memory metrics of the SAP HANA instances that are being monitored, then review the pre-configured action groups, alert rules, and alerts fired by Azure Monitor. You will also learn how to enable Azure Defender for SAP HANA VMs, configure, and enable backup for the SAP HANA database running on an Azure Virtual Machine, and how to perform an on-demand backup for the SAP HANA database and restore it.
