# Ziman Project Circle (ZPC) Marketing Material Tracker 

A Python-based inventory tracker for Ziman Project Circle (ZPC), a volunteer-run organisation without a physical office. Marketing materials and promotional items are stored by volunteers across Berlin, Hamburg, Munich and Cologne, and frequently change hands between events. The tracker provides a single source of truth for ZPC's materials: current stock per city and in total, which volunteer holds each item, and a complete history of handovers.

It supports two main use cases:

- **Monthly regional events:** event leads can see which materials are available in their city and who holds them, while every handover between volunteers is recorded, so materials can always be traced.
- **Annual conference:** the conference project manager can check existing stock across all regions before placing new orders, and record where leftover items go afterwards.

The project is developed in phases: version 1 is a terminal-based Python application; version 2 is planned as a web application accessible to coordinators in every region.

## The Problem

ZPC lacks a single source of truth for its marketing materials: stock is distributed across volunteers and moves frequently between them, yet neither current holdings nor handovers are recorded. 

ZPC operates without a central or physical office or storage facility. Marketing materials and promotional items are therefore stored at volunteer's residence in Berlin, Hamburg, Munich and Cologne. Ahead of each event or conference, volunteers and conference project managers are asked to bring the required materials to the venue. 

This creates four challenges:

- **Lack of visibility:** There is no clear record of which volunteer holds which material or in what quantities.
- **Unncessary orders before events:** Because current stock levels are unknown, new promotional items are often ordered for upcoming conferences even when sufficient stock may already exist. 
- **Untracked stock after events:** Once a conference is over, the remaining items and the volunteer who take them home are not recorded.
- **No handover tracking:** For monthly regional events, material are passed between volunteers without any record of who held them last or to whom they were handed over.

As a result, materials are occasionally unavailable at event, money is spent on duplicate orders and volunteers spend valuable time coordinating to locate items. 

The problem is made worse because volunteers and event roles change often. Volunteers join and leave ZPC, and event roles are taken by different people each month. When a volunteer leaves while still holding materials, or a new person takes over an event, nobody knows where the materials are, because this information was never written down.

## Users

**Primary Users**

- **Regional Inventory Coordinator (new role, one per region):** a new role introduced with this tracker. One volunteer in each city (Berlin, Hamburg, Munich and Cologne) is responsible for maintaining the tracker for their region, before and after events. They update it every two weeks, recording the quantity of each item, every handover between volunteers, and who currently holds the materials. The person in this role may change over time, as volunteers rotate.
- **Event Lead (monthly events):** a rotating role, taken by whichever volunteer is available or wants to lead. Each new event lead needs to quickly find out which materials exist and who currently holds them.
- **Conference Project Manager (for conferences):** prepares the materials for major conferences. Before any items are ordered, they check the current inventory, request offers from suppliers and compare prices. Once the marketing department has approved the materials, the conference project manager places the order.

**Secondary Users**

- **Volunteers:** store marketing materials at home, bring them to events and hand them over to other volunteers. Materials usually pass within the same city from one month's event to the next. For example, a volunteer in Berlin who runs the event on 20 November hands the materials to the Berlin volunteer leading the event on 20 December. Volunteers can view where stock is currently held; to get materials for an event, they contact their Regional Inventory Coordinator. Volunteers change frequently as people join, take breaks or leave ZPC.
- **Marketing Department (VP Marketing / Director):** provides ZPC's branding guidelines and, based on the conference project manager's supplier offers and price comparison, approves the branded materials for production. Uses the tracker only to view current stock levels when reviewing an order request, not to update records.

## User stories

**Regional Inventory Coordinator (RIC)**
- **RIC-01:** As a regional inventory coordinator, I want to record which materials each volunteer in my region holds and how many, so that the stock in my region is always up to date.
- **RIC-02:** As a regional inventory coordinator, I want to record every handover between volunteers (date, from, to, event and items), so that there is a complete history of who held what.
- **RIC-03:** As a regional inventory coordinator, I want to record when a volunteer leaves ZPC while still holding materials, so that those items can be collected and reassigned.
- **RIC-04:** As a regional inventory coordinator, I want to see which volunteer in my region currently holds each item, so that I can arrange handovers before each event.
- **RIC-05:** As a regional inventory coordinator, I want to add new volunteers in my region, so that I can record materials they receive.

**Event Lead (EL)**
- **EL-01:** As an event lead, I want to see which materials are available in my city and who holds them, so that I can plan my event and arrange to collect them in time.

**Conference Project Manager (CPM)**
- **CPM-01:** As a conference project manager, I want to see the total stock of each item across all regions, so that I only order what is really needed.
- **CPM-02:** As a conference project manager, I want to record newly delivered items, including new types of materials, and which volunteers receive them, so that new stock is tracked from the start.
- **CPM-03:** As a conference project manager, I want to record which volunteers take leftover items home after a conference, so that the remaining stock is not lost.

**Volunteers (VOL)**
- **VOL-01:** As a volunteer, I want to see where materials are currently held, so that I know what is available before I help at an event.

**Marketing Department (MKT)**
- **MKT-01:** As a member of the marketing department, I want to view current stock levels when reviewing an order request, so that I can confirm new materials are really needed before approving them.


## Scope

### In scope (version 1)
- Keep a list of volunteers per city, including whether they are still active.
- Keep a list of marketing materials (name, category).
- Record which volunteer holds how many of each item, and in which city.
- Record handovers between volunteers (date, from, to, city, event, items and quantities).
- Show current stock per city and total stock across all cities.
- Show the handover history, so anyone can trace who held items last.
- Mark a volunteer as having left ZPC, while still showing what they hold.
- Runs as a terminal program in Python; data is saved in files on one computer.

### Out of scope (later versions)
- A website or mobile-friendly access for coordinators in different cities (version 2).
- User accounts and different access levels (view-only vs. edit).
- Supplier offers, price comparison and order approval.
- Automatic reminders to coordinators to update the tracker.
- Low-stock alerts and reorder suggestions.
- Reports and exports for conferences.

## Tech
- Python 3
- Runs in the terminal
- Data stored in CSV files

## How to run
Coming soon.
