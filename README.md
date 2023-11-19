# Log-ingestor-and-query-interface
# Log Management System

## Overview

This project is a Log Management System consisting of a Log Ingestor and a Query Interface. It efficiently handles vast volumes of log data and provides a simple yet powerful interface for querying logs.

## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the Log Ingestor](#running-the-log-ingestor)
  - [Running the Query Interface](#running-the-query-interface)
- [System Design](#system-design)
- [Features Implemented](#features-implemented)
- [Identified Issues](#identified-issues)

## Getting Started

### Prerequisites

- Node.js and npm installed
- MongoDB installed and running locally on the default port (27017)

### Installation

1. Clone the repository:


   git clone https://github.com/Bhumikamsrit/log-management-system.git



   Navigate to the project directory:


#cd log-management-system
#Install dependencies for both the log ingestor and query interface:
npm install
#Running the Log Ingestor
node log-ingestor.js
#Running the Query Interface
node server.js
cd client
npm start
Visit http://localhost:3000 in your browser to access the Query Interface.

System Design
The system consists of two main components:

Log Ingestor:

Built with Node.js and Express.
Utilizes MongoDB for scalable and efficient log storage.
Query Interface:

Front-end built with React.
Back-end built with Node.js and Express, interacting with MongoDB for log retrieval.
Features Implemented
Log Ingestor:

Mechanism for ingesting logs in a specified format.
Scalable to handle high volumes of logs.
Mitigates bottlenecks, such as I/O operations and database write speeds.
Ingests logs via an HTTP server on port 3000.
Query Interface:

User interface (React) for full-text search across logs.
Filters based on log attributes (level, message, resourceId, timestamp, traceId, spanId, commit, metadata.parentResourceId).
Efficient search results.
Search within specific date ranges.
Utilizes regular expressions for search.
Allows combining multiple filters.
Real-time log ingestion and searching capabilities.
Role-based access control.











