---
title: Package Settings
description: See descriptions of the available package settings.
feature: Packages
exl-id: b4d415d1-86a5-40bd-b645-1709b267c174
---
# Package Settings

## Basic Details

**Name:** The package name. The maximum length is 60 characters.

**Description:** (Optional) A description of the package.

**3rd Party Billed Fees:** (Optional) A static third-party fee to be tracked as a non-billable cost:

>[!NOTE]
>
>Billable fees are reflected in the Net CPM metric.
>
* **CPM:** The cost per 1000 impressions (CPM).

* **CPM Description:** A description of the CPM fee.

You can override the package-level setting at the [placement level](/help/dsp/campaign-management/placements/placement-settings.md).

## Goals & Budget

**Pacing & Capping:** (Read-only for existing packages) At which level to pace and cap placements in the package:

* **Package level pacing:** This pacing strategy operates by pacing and capping all included placements as a *group*. This strategy ensures that all placements within a given package are optimized holistically, distributing spend based on performance and scale to selected key performance indicators (KPIs).

* **Placement level pacing:**  This pacing strategy operates by pacing and capping all included placements *individually*. The best practice is to use this strategy only to execute guaranteed private marketplace deals.

**Flight Dates:** The package's start date and end date.

To optionally create non-even pacing flights for the package, select **Activate Custom Flighting** and set up the custom flights in the Flighting section below. Once you enable custom flighting and save the package, you can't disable custom flighting.

>[!NOTE]
>
>* The flight dates must be included within the campaign flight dates. In addition, the flight dates for all placements that are assigned to this package must be included within these dates.
> * You can't edit the package start date when custom flighting is activated.

**Budget:** (Packages with package-level pacing only) The gross budget cap and the budget interval.

For packages with custom flighting, the budget interval is always *All time*. For packages without custom flighting, specify the budget interval: *All time,* *Daily,* *Monthly,* or *Weekly*.

**Gross Budget:** (Packages with package-level pacing and dynamic margin management only) The gross budget cap for all time.

**Optimization Goal:** (Packages with package-level pacing only) The optimization goal for the package. See descriptions of each optimization goal at [Optimization Goals and How to Use Them](/help/dsp/optimization/optimization-goals.md).

**Custom Goals:** (Packages with custom optimization goals only) The [custom goal](/help/dsp/optimization/custom-goal-about.md) for the package. For more information about the best practices for custom goals and campaigns that use them, see  [Best Practices for Building a Custom Goal](/help/dsp/optimization/custom-goal-best-practices.md) and [Best Practices for Setting up Performance Campaigns](/help/dsp/optimization/campaign-best-practices-performance.md).

**Package Goal Type:** (Packages with custom optimization goals only) The purpose of the package. This setting helps determine how to optimize the package:

* *Prospecting:* Prospecting packages focus on acquiring new customers.

* *Retargeting:* Retargeting packages focus on re-exposing prior visitors or customers.

* *Other:* All other purposes.

**Linked Package for Optimization Learnings Carryover:** (Packages with custom optimization goals only) Another package whose historic data is used as input for optimizing the package.

**Target:** (Packages with package-level pacing only) The target goal, which is used to track performance.

>[!NOTE]
>
>This field is only a benchmark and isn't used for decisioning.

**Frequency Cap:** (Packages with package-level pacing only) The number of times a unique device or person (depending on the specified Cross Device Level) can be served ads from the package. Options include *Unlimited* or a specific amount per day, week, or month.

>[!NOTE]
>
>* You can set frequency caps at the campaign, package, and placement levels. DSP respects the strictest frequency cap in the campaign hierarchy.
>* The best practice is to set frequency caps for both prospecting and retargeting at the package level.
> * Higher frequency caps result in higher spend and impressions but lower reach. Lower frequency caps result in lower spend and impressions but higher reach.

**Pace on:** (Packages with package-level pacing only) What pacing is based on:

* **Budget:** (Default) This option delivers as many impressions as possible within the allocated package budget.

* **Impressions:** This option delivers impressions until a specified quantity is reached within a specified interval. When you select this option, specify the number of impressions and the interval: *All time,* *Daily,* *Monthly,* or *Weekly*.

**Pacing Fill Strategy:** (Packages with package-level pacing only) How to pace ad delivery:

* *Even:* Paces delivery uniformly throughout each flight, with a target of 50% of the delivery in the first half of the flight.

* *Slightly Ahead:* (The default) Accelerates delivery so that it's 55-65% complete halfway through the flight duration.

* *Frontload:* Accelerates delivery so that it's 65-75% complete halfway through the flight.

* *Aggressive Frontload:* Accelerates delivery so that it's 75-85% complete halfway through the flight.

## Flighting

(Packages with package-level pacing and with "Activate Custom Flighting" enabled) Custom flight periods within the overall Flight Dates specified in the Goals & Budget section.

For each flight, enter the start date, end date, and the target number of impressions. To add another flight, click **Add Flight**.

>[!MORELIKETHIS]
>
>* [About Package Management](package-about.md)
>* [Create a Package](package-create.md)
>* [Edit a Package](package-edit.md)
>* [Attach a Placement to a Package](package-attach-placement.md)
>* [FAQs About Campaign Management](/help/dsp/campaign-management/campaign-management-faq.md)
