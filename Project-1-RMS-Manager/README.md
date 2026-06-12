🖥️ Project 1 — Statcon RMS Manager

Built during Internship at Statcon Electronics India Pvt. Ltd.


📌 Project Overview

The Statcon RMS Control Panel is a no-code business application built using Microsoft Power Apps, connected to Microsoft SharePoint Lists as the backend database.

The app was built to replace manual Excel-based tracking of RMS (Remote Monitoring System) modules across PCU (Power Conditioning Unit) assets — making the process faster, more accurate, and accessible from anywhere.


🎯 Problem Statement

Before this app, RMS module assignments and reconfigurations were tracked manually in Excel sheets. This caused:


Data conflicts when multiple users edited the file simultaneously
No audit trail of who changed what
No validation — wrong data could be entered easily
Not accessible on mobile or from the field
No clear visibility of asset STATUS



✅ Solution

A Power Apps application with two workflows controlled by a radio button:

WorkflowPurposeAssign New RMSRegister a brand new RMS module against a PCU assetReconfigure ModuleReassign an existing RMS from one PCU to another


🚀 Features


🔘 Radio button workflow selector — switches between Assign New RMS and Reconfigure Module
📋 Smart form — fields connected directly to SharePoint List
🔽 Specifications dropdown — 31 PCU models pre-loaded as choices
🔄 Reconfiguration dropdown — shows only PCUs with STATUS = Recycle
🔒 Read-only Previous PCU field — auto-fills from dropdown, cannot be manually edited
✅ One-click submission — data saved directly to SharePoint List
📱 Mobile accessible — works on Power Apps mobile app



🛠️ Tech Stack

ComponentTechnologyFrontendMicrosoft Power AppsDatabaseMicrosoft Lists (SharePoint)Backend ListPCU_DirectoryHostingMicrosoft 365 / SharePoint


📊 Database Structure (PCU_Directory)

ColumnTypePurposeDealer/CompanyTextDealer or company namePCU serial numberTextUnique PCU identifierSpecfications/RatingChoicePCU model (31 options)Project No./WorkorderTextAssociated projectSTATUSChoiceActive / Recycle / Pending / ReconfiguredRMS IDTextUnique RMS identifierPrevious PCUTextPCU before reconfiguration


📸 Screenshots


Screenshots of the app are available in the /Screenshots folder



