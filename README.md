# DealPilot-Salesforce-CRM
Salesforce CRM implementation project demonstrating sales process design, automation, approval workflows, reporting, and RevOps analytics.
# DealPilot Salesforce CRM

## Project Overview

DealPilot is a Salesforce CRM project that I built to simulate a real-world sales process for a software company.

The main objective of the project was to create a structured sales process in Salesforce, starting from lead management and continuing through opportunity management, approvals, automation, and reporting.

The project focuses on how Salesforce can be used not only to store customer information, but also to standardize sales processes, automate repetitive tasks, and provide visibility into sales performance.

## Business Problem

As a sales organization grows, managing leads and opportunities manually can make it difficult to maintain a consistent sales process.

For this project, I created a Salesforce setup for DealPilot where the sales team can:

* Manage leads and prospects
* Convert qualified leads into accounts, contacts, and opportunities
* Track opportunities through different sales stages
* Manage products and opportunity amounts
* Handle discount approvals
* Automate customer onboarding tasks
* Monitor pipeline and sales performance through reports and dashboards

The goal was to create a CRM process that is structured enough for sales teams while also providing useful information for management.

## Salesforce Setup

The main Salesforce objects used in the project are:

 Salesforce Object  Purpose                                                    

 Lead               Used to manage potential customers                         
 Account            Stores company or customer information                    
 Contact            Stores information about people associated with an account 
 Opportunity        Used to track potential sales and revenue                  
 Product            Represents the products being sold                         
 Task               Used for follow-ups and customer onboarding activities     

The basic lead conversion process is:

Lead → Account + Contact + Opportunity

Once a lead is converted, the opportunity can then move through the defined sales process.

## Sales Process

I created a structured opportunity process for DealPilot.

The opportunity stages used in the project are:

* Prospecting
* Qualification
* Discovery
* Demo
* Proposal
* Negotiation
* Closed Won
* Closed Lost

The purpose of defining these stages was to make it easier for the sales team to understand where each opportunity is in the buying process and for management to analyze the pipeline.

## Lead Management

Leads are used to capture potential customers before they become opportunities.

The project includes fields such as:

* Lead Name
* Company
* Email
* Phone
* Lead Source
* Lead Status

I also created a report to analyze leads by Lead Source. This helps identify which sources are generating the most leads.

When a lead is qualified, it can be converted into an Account, Contact, and Opportunity.

## Opportunity Management

Opportunities are used to track potential DealPilot sales.

The opportunity records include information such as:

* Opportunity Name
* Account
* Amount
* Stage
* Close Date
* Probability
* Products
* Opportunity Owner

The opportunity stages allow the sales team to track deals from the early stages of the sales cycle through to Closed Won or Closed Lost.

## Automation

One of the main automations in the project is related to customer onboarding.

I created a Record-Triggered Flow on the Opportunity object.

The flow is triggered when:

Stage = Closed Won

When an opportunity is marked as Closed Won, Salesforce automatically creates a Task for the customer success/onboarding team.

The task contains a message similar to:

> Customer purchased DealPilot. Please begin customer onboarding.

This demonstrates how Salesforce can be used to automate the handoff between Sales and Customer Success instead of relying on a manual follow-up.

I also created a Record-Triggered Flow on the Opportunity object to automate follow-ups when an opportunity reaches the Proposal stage.

When the opportunity stage changes to Proposal, Salesforce automatically creates a follow-up Task for the sales representative.

The task is scheduled for a few days after the opportunity enters the Proposal stage, helping the sales team follow up with prospects at the right time.

This reduces the need for manual follow-up tracking and helps ensure that opportunities do not get overlooked during the proposal stage.


## Approval Process

I also created an approval process for opportunity discounts.

The business rule used in the project is:

Discount greater than 20% → Manager approval required

The purpose of this process is to make sure that larger discounts receive the appropriate approval before the opportunity moves forward.

This also demonstrates how Salesforce can be used to enforce business rules within the sales process.

## Reports and Dashboards

I created Salesforce reports to analyze different parts of the sales process.

The reports include:

* Leads by Lead Source
* Opportunity Pipeline
* Sales Funnel
* Closed Won Opportunities
* Closed Lost Opportunities
  
The reports are intended to give sales managers visibility into pipeline value, opportunity distribution, and overall sales performance.

## Key Metrics

Some of the main sales metrics used in the project include:

* Total Pipeline
* Closed Won Revenue
* Closed Lost Revenue
* Win Rate
* Number of Opportunities
* Pipeline by Stage
* Leads by Source
* Average Opportunity Value
* Sales Funnel Conversion

These metrics can help a sales or revenue operations team understand the current state of the pipeline and identify areas that may require attention.

## Salesforce Features Used

The project uses the following Salesforce features:

* Sales Application
* Leads
* Accounts
* Contacts
* Opportunities
* Products
* Custom Opportunity Stages
* Record-Triggered Flow
* Tasks
* Approval Process
* Reports
* Dashboards
* Charts

## Project Screenshots

Screenshots of the Salesforce configuration and reports are included in the `screenshots` folder.

Some of the key screenshots include:

* DealPilot Salesforce application
* Lead management
* Lead Source report
* Opportunity records
* Opportunity pipeline
* Record-Triggered Flow
* Automated onboarding task
* Automated Proposal Follow Up
* Discount approval process
* Sales funnel
* Salesforce dashboard

## Project Documentation

The `documentation` folder contains additional information about the project, including the business requirements, Salesforce setup, automation, approval process, and reporting.

## Project Structure

DealPilot-Salesforce-CRM

* README.md
  *  screenshots
  *  dealpilot-app.png
  *  lead-management.png
  *  opportunity-pipeline.png
  *  salesforce-flow.png
  *  approval-process.png
  *  sales-funnel.png
  *  sales-dashboard.png

 * documentation
    * business-requirements.md
    * data-model.md
    * automation.md
    * approval-process.md
    * reports-and-dashboards.md

## What I Learned

This project gave me practical experience with Salesforce configuration and helped me understand how CRM functionality connects with actual sales operations.

Some of the key areas I worked on were:

* Designing a sales process
* Managing leads and opportunities
* Understanding lead conversion
* Configuring Salesforce objects and fields
* Creating Salesforce Flow automation
* Creating approval processes
* Building sales reports
* Creating sales funnel and pipeline reports
* Using CRM data to understand sales performance

## Project Information

**Project:** DealPilot Salesforce CRM

**Platform:** Salesforce

**Focus:** CRM Operations, Sales Operations, Revenue Operations, Automation and Sales Analytics
