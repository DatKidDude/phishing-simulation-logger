# Project Objectives

Simulate a phishing email campaign in a controlled environment to understand how users interact with suspicious links, and to analyze the type of data that can be captured when a target clicks on a phishing link.

## Goals

- Create a fake phishing email with a link to a controlled domain
- Log user interactions upon clicking the phishing link
- Analyze and report on the information collected
- Collect Data
  - Timestamp
  - IP address
  - User-Agent
  - Screen size
  - Screen resolution
  - Browser language

## Languages Used

- Python
- HTML
- CSS
- Javascript

## Phase 1: Design the phishing email

**Goal**: Design a plausible phishing email

1. Will start out with just a link until I get the website running

## Phase 1.5: Build email server

**Goal**: Design an email server to send out phishing email

1. (1.5) Use smtplib to send out the email template

## Phase 2: Build the Local Server

**Goal**: Create the backend that logs information

2. Setup a local server using Flask
3. Create a route like `/click` to log data:
   - All request headers
   - URL parameters
   - JS-collected data (sent via `fetch()` or form)
4. Print data to landing page

## Phase 3: Frontend (Phishing Page)

**Goal**: Make a fake landing page

5. Design the HTML page
   - Create a landing page that prints all the collected data
6. Add Javascript to log extra info
   - Example: screen resolution, platform, language
   - Send data back to server (via `fetch()` or form POST)

## Phase 4: Testing

**Goal**: Try it out locally

5. Click my own link from different browsers/devices (VM's)
   - Check what's logged
   - Make sure query parameters work
   - Confirm logging format
