# Ziman Project Circle (ZPC) Marketing Material Tracker 

A Python-based inventory tracker for Ziman Project Circle (ZPC), a volunteer-run organisation without a physical office. Marketing materials and promotional items are stored by volunteers across Berlin, Hamburg, Munich and Cologne, and frequently change hands between events. The tracker provides a single source of truth for ZPC's materials: current stock per city and in total, which volunteer holds each item, and a complete history of handovers.

It supports two main use cases:

- **Monthly regional events:** event leads can see which materials are available in their city and who holds them, while every handover between volunteers is recorded, so materials can always be traced.
- **Annual conference:** the conference project manager can check existing stock across all regions before placing new orders, and record where leftover items go afterwards.

The project is developed in phases: version 1 is a terminal-based Python application; version 2 is planned as a web application accessible to coordinators in every region.

## The Problem

ZPC lacks a single source of truth for its marketing materials: stock is distributed across volunteers and moves frequently between them, yet neither current holdings nor handovers are recorded. 

ZPC operates without a central office or storage facility. Marketing materials and promotional items are therefore stored at volunteer's homes in Berlin, Hamburg, Munich and Cologne. Ahead of each event or conference, volunteers are asked to bring the required materials to the venue. 

This creates four challenges:

- **Lack of visibility:** There is no clear record of which volunteer holds which material or in what quantities.
- **Unncessary orders before events:** Because current stock levels are unknown, new promotional items are often ordered for upcoming conferences even when sufficient stock may already exist. 
- **Untracked stock after events:** Once a conference is over, the remaining items and the volunteer who take them home are not recorded.
- **No handover tracking:** For weekly and monthly regional events, material are passed between volunteers without any record of who held them last or to whom they were handed over.

As a result, materials are occasionally unavailable at event, money is spent on duplicate orders and volunteers spend valuable time coordinating to locate items. 

## Users

**Primary Users**

- **Volunteers:** store marketing materials at home, bring them to events and hand them over to other volunteers. Material usually pass within the same city from one month's event to the next. For example, a volunteer in Berlin who runs the event on 20 November hands the material to the Berlin volunteer leading the event on 20 December. Volunteers change frequently as people join, take breaks or leave ZPC.
- **Event Lead (monthly events):** A rotating role, taken by whichever volunteer is available or wants to lead. Each new event lead needs to quickly fidn out which materials exist and who currently holds them.
- **Conference Project Manager (for conference):** Prepares the materials for major conferences. Before any items are ordered, they check the current inventory, request offers from suppliers and compare prices. Once the marketing department has approved the material, the conference project manger places the order.

**Secondary Users**

- **Marketing Department (VP Marketing/Director)** provides ZPC's branding guidelines and based on the conference project manager 's suppliers offers and price comparison approves the branding materials for production. Uses the tracker only to view current stock levels when reviewing an order request, not to update records. 
