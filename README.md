## 📅 Releases Working Group Calendar Website

- Name: Daulet Zharassar
- Email: dauletjarasar@gmail.com
- Github: [ZhQriks](https://github.com/zhqriks)
- Location: Kazakhstan, Almaty
- Time Zone: UTC+5
- School: Nazarbayev intellectual school of physics and mathematics in Astana
- Major: Computer science

**Project Description**
=====================
- Name: [📅 Releases Working Group Calendar Website](https://ccextractor.org/public/gsoc/rtorrent-modern-rpc/)
- Mentors: [@dsanders11](https://github.com/dsanders11), [@vertedinde](https://github.com/vertedinde)
- Synopsis:
  The Electron Release Working Group currently relies on several disparate automated tracks to track and communicate details about major **Electron** stable releases. This project aims to streamline this process by creating a release calendar website that will pull dates from the **Chromium API** and display them in a user-friendly manner. The website will be built using **React**. Additional information will be added to Slack using a bot built on the **Slack API**, notifying and editing via the **#wg-releases** channel


**About me**
=====================
Hi I am Zharasar from Kazakhstan, This year I am finishing 12th grade in high school. My main programming language is Javascript. I started at the age of 15 by creating simple applications interacting with DOM. Now at the age of 18 I develop complex projects using React & Typescript.

For 1.5 years I've been working at Owl Tribe outsourcing company where I've worked on 5+ projects including Electron, React-Native, Nextjs, Django. I enjoy to participate in coding competitions, and have already won 10 hackathons. My latest project is Nodemap - AI Roadmap Generator. [Link](https://nodemap.vercel.app).


**Diagram**
=====================
![electron-diagram](https://github.com/ZhQriks/gsoc-proposal/assets/49629027/d0148844-fa7d-411c-b124-72489d9e3205)


A simple diagram describing my vision of process integration for this project

## Deliverables:

1. ### React website to monitor team beta and stable release dates:
   - Prerequisites for the project
   - Receiving data from the express server
   - Coding a custom component for a calendar
   - Style the components using CSS

2. ### Express server modifications:
   - Fetching release data from the Chromium API
   - Storage of fetched data
   - Implement data syncing with the Slack
   - Endpoints for the React website

3. ### Documentation for **Releases Working Group Calendar**:
   - Create user guides for the React website, explaining how to navigate and use the features
   - Provide documentation for the Slack bot, including instructions on how to install and use the bot

4. ### Slack Bot
   - Notifications of new calendar changes in slack
   - Interactive commands for manual change of information
   - Interaction with express


**Detailed Description**
=====================
The React website will provide a user-friendly interface for monitoring release dates, while the modified Express server will handle data fetching and syncing. The Slack bot integration will enable seamless notifications and interactive commands, making collaboration and communication better within the Releases Working Group.


1. ### Creating a React Calendar Website
   - **Problem:** The Releases Working Group needs a user-friendly website to monitor team beta and stable release dates.
   - **Solution:**
     - Typescript initialization
     - Create a React website with two pages: a main page with a custom calendar component and a detailed release details page.
     - Use the `node-fetch` library to fetch data from the modified electron-release Express server.
     - Implement a custom `<Calendar {...} />` component to display release dates and events.
     - Style the components using CSS to ensure an attractive and intuitive user interface.

2. ### Express Server Modifications
   - **Problem:** The existing electron-release Express server needs to be modified to fetch and store release data from the Chromium API and sync with Slack.
   - **Solution:**
     - Modify the Express server to fetch release updates from the Chromium API on a scheduled basis.
       - Use a library like node-cron to create a non-blocking synchronous task.
       - Define the schedule for the task (e.g., every hour, every day at a specific time). 
     - Implement data storage functionality to store the fetched release data.
     - Develop endpoints for the React website to access the stored release data.
     - Integrate data syncing functionality with Slack using the Slack API.
       - Use the `@slack/web-api` library to interact with the Slack API.
       - Authenticate the Express server with the Slack API using the obtained API token.
       - Implement functions to send release data updates to the **#wg-releases** Slack channel.
       - Set up a scheduled task or trigger to automatically sync release data with Slack at regular intervals.

3. ### Slack Bot Integration
   - **Problem:** The Releases Working Group needs a Slack bot to provide notifications and interact with the release data.
   - **Solution:**
     - Create and configure a Slack bot using the Slack API and obtain an API token.
     - Integrate the Slack bot within the Express app, likely within the existing electron-release repository.
     - Implement functionality for the Slack bot to notify **#wg-releases** Slack channel when a new release is fetched using the `@slack/events-api` library.
     - Develop interactive commands for the Slack bot using the Block Kit UI Framework, allowing users to:
       - List releases
       - Show the latest release
       - Create new Electron releases
       - Edit release information

**Brief Timeline**
=====================

- **before May 20**
  - communicate with mentor to understand and details the goal of project;
  - research and familiarize with the Electron release process and existing electron-release repository

- **May 21 - June 12**
  - set up development environment for React website and Express server modifications
  - create basic structure of the React website with components
  - modify Express server to fetch release data from the Chromium API and implement data storage
  - stablish communication between the React website and Express server to retrieve release data

- **June 13 - July 25**
  - develop custom calendar component in React to display release dates and events
  - implement detailed release details page in the React website
  - integrate Slack API into the Express server for data syncing
  - develop endpoints in the Express server for the React website to access release data
  - create and configure the Slack bot for notifications and interactive commands

- **July 26 - August 4**
  - integrate the Slack bot with the Express server
  - implement notification functionality for new release updates
  - develop interactive commands for the Slack bot (list releases, show latest release, create new releases, edit release information)
  - conduct thorough testing of the React website, Express server, and Slack bot integration

- **August 5 - September 4**
  - gather team feedback and iterate on the React website and Slack bot based on the feedback received
  - fine-tune the user interface and user experience of the React website
  - create user guides and documentation for the React website and Slack bot

- **September 5 - September 12**
  - code style and quality review, dev documentation
  - prepare for final evaluation

**Why me**
=====================
I self-taught became a developer at the early age of 15.  During this time I found an unrivaled passion for programming. I like to understand complex concepts and do the work quickly to get more feedback

When I was 15 years old and entered the Desktop Application Contest as a Web Developer, my eyes fell on Electron and when I entered the contest I transferred my project to desktop in just 5 minutes. Since that day I still find Electron to be magical and empowering for thousands of web developers
